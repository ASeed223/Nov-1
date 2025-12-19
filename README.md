---
- name: Upgrade Nexus Repository Manager (Step 1: Find, Extract & Archive)
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
        owner: nexus
        group: nexus
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
