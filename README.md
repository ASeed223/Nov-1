---
- name: Test Configuration Only (nexus.vmoptions & jetty-https.xml)
  hosts: lxpd208
  gather_facts: no
  vars_prompt:
    - name: "target_version"
      prompt: "Enter target version (e.g. 3.86)"
      private: no

  vars:
    nexus_root: "/opt/nexus"
    # Hardcoded password for testing; will be encrypted later
    hardcoded_password: "OBF:123789Qw#"

  tasks:
    # ==========================================================================
    # 1. Locate Directory (Logic: Find -> Calculate Path)
    # ==========================================================================
    - name: "Find Nexus tarball to identify version directory"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*.tar.gz"
      register: nexus_tarballs

    - name: "Fail if no tarball found"
      ansible.builtin.fail:
        msg: "No tarball found for version {{ target_version }}"
      when: nexus_tarballs.matched == 0

    - name: "Set directory facts"
      ansible.builtin.set_fact:
        nexus_tarball_name: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path | basename }}"

    - name: "Calculate directory path"
      ansible.builtin.set_fact:
        # Logic: nexus-3.86.2-01-unix.tar.gz -> nexus-3.86.2-01
        new_nexus_dir: "{{ nexus_root }}/{{ (nexus_tarball_name | regex_replace('(-unix|-linux-x86_64)?\\.tar\\.gz$', '')) }}"

    - name: "Confirm Target Directory"
      ansible.builtin.debug:
        msg: "Testing configuration on: {{ new_nexus_dir }}"

    # ==========================================================================
    # 2. Configure nexus.vmoptions
    # ==========================================================================
    - name: "Update Memory Settings (6G)"
      ansible.builtin.lineinfile:
        path: "{{ new_nexus_dir }}/bin/nexus.vmoptions"
        regexp: "{{ item.regex }}"
        line: "{{ item.line }}"
      loop:
        - { regex: '^-Xms', line: '-Xms6G' }
        - { regex: '^-Xmx', line: '-Xmx6G' }
        - { regex: '^-XX:MaxDirectMemorySize=', line: '-XX:MaxDirectMemorySize=15530M' }

    - name: "Update Data & Log Paths"
      ansible.builtin.lineinfile:
        path: "{{ new_nexus_dir }}/bin/nexus.vmoptions"
        regexp: "{{ item.regex }}"
        line: "{{ item.line }}"
      loop:
        - { regex: '^-Dkaraf.data=', line: '-Dkaraf.data=/opt/nexus/sonatype-work/nexus3' }
        - { regex: '^-Dkaraf.log=', line: '-Dkaraf.log=/opt/nexus/sonatype-work/nexus3/log' }
        - { regex: '^-Djava.io.tmpdir=', line: '-Djava.io.tmpdir=/opt/nexus/sonatype-work/nexus3/tmp' }
        - { regex: '^-XX:LogFile=', line: '-XX:LogFile=/opt/nexus/sonatype-work/nexus3/log/jvm.log' }

    # ==========================================================================
    # 3. Configure jetty-https.xml
    # ==========================================================================
    - name: "Update KeyStorePassword"
      ansible.builtin.replace:
        path: "{{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
        # Regex: Capture <Set...>, capture </Set>, replace the middle part
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
        # Note: TrustStorePassword tag has 'property' attribute, so we use .*
        regexp: '(<Set name="TrustStorePassword".*>)(.*)(</Set>)'
        replace: '\1{{ hardcoded_password }}\3'

    # ==========================================================================
    # 4. Completion Summary
    # ==========================================================================
    - name: "Test Complete"
      ansible.builtin.debug:
        msg: 
          - "Configuration Updated."
          - "Please check: {{ new_nexus_dir }}/bin/nexus.vmoptions"
          - "Please check: {{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
