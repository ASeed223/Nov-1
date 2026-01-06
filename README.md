---
- name: Nexus Full Upgrade - Stop, Link, and Start
  hosts: lxpd208
  gather_facts: no
  any_errors_fatal: true
  vars_prompt:
    - name: "target_version"
      prompt: "Enter target version (e.g. 3.87)"
      private: no

  vars:
    nexus_root: "/opt/nexus"
    nexus_link: "/opt/nexus/nexus"
    hardcoded_password: "OBF:123789"

  tasks:
    # --- STEP 1: PREPARATION ---
    - name: "Find Nexus tarball for version {{ target_version }}"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*.tar.gz"
      register: nexus_tarballs

    - name: "Fail if tarball is missing"
      ansible.builtin.fail:
        msg: "No tarball found for version {{ target_version }}"
      when: nexus_tarballs.matched == 0

    - name: "Set version and directory variables"
      ansible.builtin.set_fact:
        nexus_tarball: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path }}"
        extracted_dir_name: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path | basename | regex_replace('(-unix|-linux-x86_64)?\\.tar\\.gz$', '') }}"

    - name: "Define new directory path"
      ansible.builtin.set_fact:
        new_nexus_dir: "{{ nexus_root }}/{{ extracted_dir_name }}"

    - name: "Extract new Nexus version"
      ansible.builtin.unarchive:
        src: "{{ nexus_tarball }}"
        dest: "{{ nexus_root }}"
        remote_src: yes
        creates: "{{ new_nexus_dir }}"

    # --- STEP 2: STOP OLD SERVICE ---
    - name: "Check if a Nexus process is currently active"
      ansible.builtin.shell: ps -ef | grep java | grep "{{ nexus_link }}" | grep -v grep
      register: process_check
      failed_when: false
      changed_when: false

    - name: "Stop existing Nexus service"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus stop"
      when: process_check.rc == 0
      failed_when: false # Prevent failure if PID file is already missing

    - name: "Wait for process to terminate"
      ansible.builtin.shell: ps -ef | grep java | grep "{{ nexus_link }}" | grep -v grep
      register: verify_stop
      until: verify_stop.rc != 0
      retries: 15
      delay: 5
      failed_when: false

    # --- STEP 3: CONFIGURE NEW VERSION ---
    - name: "Apply JVM configurations to the new directory"
      ansible.builtin.lineinfile:
        path: "{{ new_nexus_dir }}/bin/nexus.vmoptions"
        regexp: "{{ item.regex }}"
        line: "{{ item.line }}"
      loop:
        - { regex: '^-Xms', line: '-Xms6G' }
        - { regex: '^-Xmx', line: '-Xmx6G' }
        - { regex: '^-XX:MaxDirectMemorySize=', line: '-XX:MaxDirectMemorySize=15530M' }
        - { regex: '^-Dkaraf.data=', line: '-Dkaraf.data=/opt/nexus/sonatype-work/nexus3' }
        - { regex: '^-Dkaraf.log=', line: '-Dkaraf.log=/opt/nexus/sonatype-work/nexus3/log' }
        - { regex: '^-Djava.io.tmpdir=', line: '-Djava.io.tmpdir=/opt/nexus/sonatype-work/nexus3/tmp' }
        - { regex: '^-Djava.net.preferIPv4Stack=', line: '-Djava.net.preferIPv4Stack=true' }

    - name: "Apply SSL configurations to the new directory"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        regexp: "{{ item.regexp }}"
        replace: "{{ item.replace }}"
      loop:
        - { regexp: '(<Property name="jetty.sslContext.keyStorePath" default=")(.*)(" />)', replace: '\1nexus01.jks\3' }
        - { regexp: '(<Set name="KeyStorePassword">)(.*)(</Set>)', replace: '\1{{ hardcoded_password }}\3' }

    # --- STEP 4: SWITCH SOFTLINK & VERIFY ---
    - name: "Update softlink to point to the new version"
      ansible.builtin.file:
        src: "{{ new_nexus_dir }}"
        dest: "{{ nexus_link }}"
        state: link
        force: yes

    - name: "Verify softlink points to the correct version"
      ansible.builtin.stat:
        path: "{{ nexus_link }}"
      register: link_stat

    - name: "Assert link target contains target version"
      ansible.builtin.assert:
        that:
          - "target_version in link_stat.stat.lnk_source"
        fail_msg: "Link verification failed! Points to {{ link_stat.stat.lnk_source }}"

    # --- STEP 5: START NEW SERVICE & HEALTH CHECK ---
    - name: "Start Nexus (New Version)"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus start"

    - name: "Wait for API Health Check (HTTP 200)"
      ansible.builtin.shell: "curl -k -s -o /dev/null -w '%{http_code}' https://127.0.0.1:8443/service/rest/v1/status"
      register: health_check
      until: health_check.stdout == "200"
      retries: 20
      delay: 10
      failed_when: false

    - name: "Trigger Auto-Heal if first start failed"
      block:
        - name: "Auto-Heal: Restarting Nexus"
          ansible.builtin.shell: "{{ nexus_link }}/bin/nexus restart"
        - name: "Auto-Heal: Final Health Check"
          ansible.builtin.shell: "curl -k -s -o /dev/null -w '%{http_code}' https://127.0.0.1:8443/service/rest/v1/status"
          register: final_check
          until: final_check.stdout == "200"
          retries: 15
          delay: 10
      when: health_check.stdout != "200"

    # --- STEP 6: CLEANUP ---
    - name: "Move tarball to archive"
      ansible.builtin.command: "mv {{ nexus_tarball }} {{ nexus_root }}/archive/"
      args:
        removes: "{{ nexus_tarball }}"

    - name: "Completion Summary"
      ansible.builtin.debug:
        msg: "Nexus upgraded to {{ target_version }} and service is verified UP."
