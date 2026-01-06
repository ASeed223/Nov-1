---
- name: Upgrade Nexus HA
  hosts: lxpd208
  gather_facts: no
  vars_prompt:
    - name: "target_version"
      prompt: "Enter target version (e.g. 3.86)"
      private: no

  tasks:
    - name: "Set Nexus root path"
      ansible.builtin.set_fact:
        nexus_root: "/opt/nexus"

    # --- 1. Find Tarball ---
    - name: "Find Nexus tarball for version {{ target_version }}"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*.tar.gz"
        recurse: no
        file_type: file
      register: nexus_tarballs

    - name: "Fail if no tarball found"
      ansible.builtin.fail:
        msg: "No Nexus tarball found for version {{ target_version }} in {{ nexus_root }}"
      when: nexus_tarballs.matched == 0

    - name: "Pick latest tarball by mtime"
      ansible.builtin.set_fact:
        nexus_tarball: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path }}"
        nexus_tarball_name: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path | basename }}"

    - name: "Display selected tarball"
      ansible.builtin.debug:
        msg: "Found: {{ nexus_tarball }}"

    # --- 2. Calculate Directory Name ---
    - name: "Extract expected directory name from filename"
      ansible.builtin.set_fact:
        # Remove .tar.gz and suffixes to get folder name (e.g., nexus-3.86.0-01)
        extracted_dir_name: "{{ nexus_tarball_name | regex_replace('(-unix|-linux-x86_64)?\\.tar\\.gz$', '') }}"

    - name: "Set full path for the new release"
      ansible.builtin.set_fact:
        new_nexus_dir: "{{ nexus_root }}/{{ extracted_dir_name }}"

    # --- 3. Extract ---
    - name: "Extract Nexus tarball"
      ansible.builtin.unarchive:
        src: "{{ nexus_tarball }}"
        dest: "{{ nexus_root }}"
        remote_src: yes
        creates: "{{ new_nexus_dir }}"

    # --- 4. Archive ---
    - name: "Ensure archive directory exists"
      ansible.builtin.file:
        path: "{{ nexus_root }}/archive"
        state: directory
        mode: '0755'

    - name: "Move tarball to archive folder"
      ansible.builtin.command:
        cmd: "mv {{ nexus_tarball }} {{ nexus_root }}/archive/"
      args:
        # Only run if file exists (prevents error on re-run)
        removes: "{{ nexus_tarball }}"

    - name: "Display Archive Result"
      ansible.builtin.debug:
        msg: "Moved {{ nexus_tarball_name }} to {{ nexus_root }}/archive/"




        
---
- name: Test Configuration Only (Safe Edit Strategy)
  hosts: lxpd208
  gather_facts: no
  vars_prompt:
    - name: "target_version"
      prompt: "Enter target version (e.g. 3.87)"
      private: no

  vars:
    nexus_root: "/opt/nexus"
    hardcoded_password: "OBF:123789"

  tasks:
    # 1. Find Directory
    - name: "Find existing Nexus directory matching version {{ target_version }}"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*"
        file_type: directory
        recurse: no
      register: nexus_dirs

    - name: "Fail if no directory found"
      ansible.builtin.fail:
        msg: "No directory found for version {{ target_version }} in {{ nexus_root }}"
      when: nexus_dirs.matched == 0

    - name: "Set target directory path"
      ansible.builtin.set_fact:
        # Sort by mtime to pick the latest folder
        new_nexus_dir: "{{ (nexus_dirs.files | sort(attribute='mtime') | last).path }}"

    - name: "Confirm Target Directory"
      ansible.builtin.debug:
        msg: "Testing configuration on: {{ new_nexus_dir }}"

    # 2. Configure nexus.vmoptions
    # Strategy: Keep defaults, modify specific values, append if missing
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
        
        # Restore missing flags (Appends to end of file if not found)
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

    # 4. Summary
    - name: "Test Complete"
      ansible.builtin.debug:
        msg: 
          - "Configuration Updated."
          - "Please check: {{ new_nexus_dir }}/bin/nexus.vmoptions (Check end of file for IPv4 flag)"
          - "Please check: {{ new_nexus_dir }}/etc/jetty/jetty-https.xml"
