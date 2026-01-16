- name: Nexus_HA_Full_Automated_Upgrade
  hosts: lxpd208
  gather_facts: no
  any_errors_fatal: true

  vars_prompt:
    - name: "target_version"
      prompt: "Enter target version (e.g. 3.87.1)"
      private: no

  vars:
    nexus_root: "/opt/nexus"
    nexus_link: "/opt/nexus/nexus"
    hardcoded_password: "OBF:123"
    secondary_node: "lxpd209"

  tasks:
    # PHASE 1: Preparation and Config lxpd208
    - name: "Find Nexus tarball on lxpd208"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*.tar.gz"
      register: nexus_tarballs

    - name: "Fail if tarball is missing"
      ansible.builtin.fail:
        msg: "No tarball found for version {{ target_version }}"
      when: nexus_tarballs.matched == 0

    - name: "Set version and path facts"
      ansible.builtin.set_fact:
        nexus_tarball: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path }}"
        extracted_dir_name: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path | basename | regex_replace('(-unix|-linux-x86_64)?\\.tar\\.gz$', '') }}"

    - name: "Define new directory path"
      ansible.builtin.set_fact:
        new_nexus_dir: "{{ nexus_root }}/{{ extracted_dir_name }}"

    - name: "Extract Nexus on lxpd208"
      ansible.builtin.unarchive:
        src: "{{ nexus_tarball }}"
        dest: "{{ nexus_root }}"
        remote_src: yes
        creates: "{{ new_nexus_dir }}"

    # 2. Configure nexus.vmoptions
    - name: "Update vmoptions (Memory, Paths, and Missing Flags)"
      ansible.builtin.lineinfile:
        path: "{{ new_nexus_dir }}/bin/nexus.vmoptions"
        regexp: "{{ item.regex }}"
        line: "{{ item.line }}"
      loop:
        # Memory Settings
        - { regex: '^-Xms', line: '-Xms6G' }
        - { regex: '^-Xmx', line: '-Xmx6G' }
        - { regex: '^-XX:MaxDirectMemorySize=', line: '-XX:MaxDirectMemorySize=15530M' }
        
        # Path Settings
        - { regex: '^-Dkaraf.data=', line: '-Dkaraf.data=/opt/nexus/sonatype-work/nexus3' }
        - { regex: '^-Dkaraf.log=', line: '-Dkaraf.log=/opt/nexus/sonatype-work/nexus3/log' }
        - { regex: '^-Djava.io.tmpdir=', line: '-Djava.io.tmpdir=/opt/nexus/sonatype-work/nexus3/tmp' }
        - { regex: '^-XX:LogFile=', line: '-XX:LogFile=/opt/nexus/sonatype-work/nexus3/log/jvm.log' }
        
        # Restore missing flags
        - { regex: '^-Djava.net.preferIPv4Stack=', line: '-Djava.net.preferIPv4Stack=true' }
        - { regex: '^-Dkaraf.startLocalConsole=', line: '-Dkaraf.startLocalConsole=false' }

    # 3. Configure jetty-https.xml
    - name: "Update KeyStorePath to nexus01.jks"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        regexp: '(<Property name="jetty.sslContext.keyStorePath" default=")(.*)(" />)'
        replace: '\1nexus01.jks\3'

    - name: "Update KeyStorePassword"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        regexp: '(<Set name="KeyStorePassword">)(.*)(</Set>)'
        replace: '\1{{ hardcoded_password }}\3'

    - name: "Update KeyManagerPassword"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        regexp: '(<Set name="KeyManagerPassword">)(.*)(</Set>)'
        replace: '\1{{ hardcoded_password }}\3'

    - name: "Update TrustStorePassword"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        regexp: '(<Set name="TrustStorePassword".*>)(.*)(</Set>)'
        replace: '\1{{ hardcoded_password }}\3'

    # PHASE 2: REPLICATION TO lxpd209
    - name: "Sync configured folder to {{ secondary_node }} using rsync"
      ansible.builtin.shell: "rsync -avzP {{ new_nexus_dir }}/ {{ secondary_node }}:{{ new_nexus_dir }}/"
      register: rsync_result

    # PHASE 3: UPGRADE lxpd208
    - name: "[lxpd208] Stop service"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus stop"
      failed_when: false

    - name: "[lxpd208] Wait for process to exit"
      ansible.builtin.shell: ps -ef | grep java | grep "org.sonatype.nexus.bundle.Main" | grep -v grep
      register: wait_stop_208
      until: wait_stop_208.rc != 0
      retries: 12
      delay: 5
      failed_when: false

    - name: "[lxpd208] Update softlink to {{ target_version }}"
      ansible.builtin.file:
        src: "{{ new_nexus_dir }}"
        dest: "{{ nexus_link }}"
        state: link
        force: yes

    - name: "[lxpd208] Start new service"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus start"

    - name: "[lxpd208] Health Check (Wait for HTTP 200)"
      ansible.builtin.uri:
        url: "https://127.0.0.1:8443/service/rest/v1/status"
        validate_certs: no
        status_code: 200
      register: health_208
      until: health_208.status == 200
      retries: 20
      delay: 10
      ignore_errors: yes

    # PHASE 4: UPGRADE lxpd209
    - name: "[lxpd209] Stop service"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus stop"
      delegate_to: "{{ secondary_node }}"
      failed_when: false

    - name: "[lxpd209] Wait for process to exit"
      ansible.builtin.shell: ps -ef | grep java | grep "org.sonatype.nexus.bundle.Main" | grep -v grep
      delegate_to: "{{ secondary_node }}"
      register: wait_stop_209
      until: wait_stop_209.rc != 0
      retries: 12
      delay: 5
      failed_when: false

    - name: "[lxpd209] Update softlink to {{ target_version }}"
      ansible.builtin.file:
        src: "{{ new_nexus_dir }}"
        dest: "{{ nexus_link }}"
        state: link
        force: yes
      delegate_to: "{{ secondary_node }}"

    - name: "[lxpd209] Start new service"
      ansible.builtin.shell: "{{ nexus_link }}/bin/nexus start"
      delegate_to: "{{ secondary_node }}"

    - name: "[lxpd209] Health Check (Wait for HTTP 200)"
      ansible.builtin.uri:
        url: "https://{{ secondary_node }}:8443/service/rest/v1/status"
        validate_certs: no
        status_code: 200
      register: health_209
      until: health_209.status == 200
      retries: 20
      delay: 10
      ignore_errors: yes

    # PHASE 5: CLEANUP
    - name: "Move tarball to archive folder on lxpd208"
      ansible.builtin.command: "mv {{ nexus_tarball }} {{ nexus_root }}/archive/"
      args:
        removes: "{{ nexus_tarball }}"

    - name: "Final Summary"
      ansible.builtin.debug:
        msg: 
          - "Upgrade to {{ target_version }} completed successfully."
          - "Primary (lxpd208) status: {{ health_208.status | default('Failed') }}"
          - "Secondary (lxpd209) status: {{ health_209.status | default('Failed') }}"
