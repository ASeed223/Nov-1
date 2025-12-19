---
- name: Upgrade Nexus IQ Server
  hosts: lxpd196
  gather_facts: no

  tasks:
    - name: "Set IQ version from extra vars"
      ansible.builtin.set_fact:
        iq_version: "{{ iq_version }}"

    - name: "Set Nexus root path"
      ansible.builtin.set_fact:
        nexus_root: "/opt/appdata/nexus"

    # Find the tar.gz file containing the full version string
    - name: "Find IQ tarball for version {{ iq_version }}"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ iq_version }}*.tar.gz"
        recurse: no
        file_type: file
      register: iq_tarballs

    - name: "Fail if no tarball found for version {{ iq_version }}"
      ansible.builtin.fail:
        msg: "No IQ tarball found for version {{ iq_version }} in {{ nexus_root }}"
      when: iq_tarballs.matched == 0

    - name: "Pick latest tarball by mtime"
      set_fact:
        iq_tarball: "{{ (iq_tarballs.files | sort(attribute='mtime') | last).path }}"

    # Extract full version from tarball filename (e.g. 1.193.0-01)
    - name: "Extract full version string from tarball filename"
      set_fact:
        full_version: >-
          {{ (iq_tarball | basename).split('-bundle.tar.gz')[0].split('nexus-iq-server-')[-1] }}

    - name: "Create target directory nexus-iq-server-{{ full_version }}"
      ansible.builtin.file:
        path: "{{ nexus_root }}/nexus-iq-server-{{ full_version }}"
        state: directory

    - name: "Extract IQ tarball into versioned directory"
      ansible.builtin.unarchive:
        src: "{{ iq_tarball }}"
        dest: "{{ nexus_root }}/nexus-iq-server-{{ full_version }}"
        remote_src: yes
        extra_opts: ["--strip-components=0"]

    - set_fact:
        new_iq_dir: "{{ nexus_root }}/nexus-iq-server-{{ full_version }}"

    # Read the current symlink
    - name: "Get current nexus-iq-server symlink"
      ansible.builtin.stat:
        path: "{{ nexus_root }}/nexus-iq-server"
        follow: false
      register: iq_symlink

    - set_fact:
        current_iq_dir: "{{ iq_symlink.stat.lnk_target }}"

    # Copy config.yml from old to new version
    - name: "Copy config.yml to new version"
      ansible.builtin.copy:
        src: "{{ current_iq_dir }}/config.yml"
        dest: "{{ new_iq_dir }}/config.yml"
        remote_src: yes

    # Update the symlink to point to new version
    - name: "Update symlink to new version"
      ansible.builtin.file:
        path: "{{ nexus_root }}/nexus-iq-server"
        src: "{{ new_iq_dir }}"
        state: link
        force: yes

    # Restart the IQ Server using fixed path
    - name: Stop Nexus IQ Server
      ansible.builtin.shell: /opt/appdata/nexus/restart-iq-server stop
      register: stop_iq
      changed_when: stop_iq.rc == 0
      failed_when: stop_iq.rc != 0

    - name: Wait until Nexus IQ Server process disappears
      ansible.builtin.shell: |
        set -o pipefail
        ps -ef | grep '[j]ava' | grep 'nexus-iq-server' > /dev/null
      register: proc_check
      changed_when: false
      failed_when: false 
      retries: 6              
      delay: 5
      until: proc_check.rc != 0  

    - name: Fail if Nexus IQ Server is still running
      ansible.builtin.fail:
        msg: "Nexus IQ Server failed to stop on {{ inventory_hostname }}!"
      when: proc_check.rc == 0 

    - name: Wait 10 seconds
      ansible.builtin.pause:
        seconds: 10

    - name: Start Nexus IQ Server
      ansible.builtin.shell: /opt/appdata/nexus/restart-iq-server start
      register: start_iq
      changed_when: start_iq.rc == 0
      failed_when: start_iq.rc != 0

    - name: Wait until Nexus IQ Server process appears
      ansible.builtin.shell: |
        set -o pipefail
        ps -ef | grep '[j]ava' | grep 'nexus-iq-server' > /dev/null
      register: proc_check
      changed_when: false
      failed_when: false
      retries: 6             
      delay: 5
      until: proc_check.rc == 0  

    - name: Fail if Nexus IQ Server failed to start
      ansible.builtin.fail:
        msg: "Nexus IQ Server failed to start on {{ inventory_hostname }}!"
      when: proc_check.rc != 0

    # Remove tar.gz after successful deployment
    - name: Remove tarball {{ iq_tarball }} after deployment
      ansible.builtin.file:
        path: "{{ iq_tarball }}"
        state: absent
