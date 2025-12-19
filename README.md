---
- name: Upgrade Nexus Repository Manager (Step 1: Find & Extract)
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

    # 1. Find the tarball matching the input version
    - name: "Find Nexus tarball for version {{ target_version }}"
      ansible.builtin.find:
        paths: "{{ nexus_root }}"
        patterns: "*{{ target_version }}*.tar.gz"
        recurse: no
        file_type: file
      register: nexus_tarballs

    - name: "Fail if no tarball found for version {{ target_version }}"
      ansible.builtin.fail:
        msg: "No Nexus tarball found for version {{ target_version }} in {{ nexus_root }}"
      when: nexus_tarballs.matched == 0

    - name: "Pick latest tarball by mtime"
      ansible.builtin.set_fact:
        nexus_tarball: "{{ (nexus_tarballs.files | sort(attribute='mtime') | last).path }}"

    - name: "Display selected tarball"
      ansible.builtin.debug:
        msg: "Selected tarball: {{ nexus_tarball }}"

    # 2. Calculate the directory name that will be created
    # Logic: nexus-3.86.2-01-unix.tar.gz -> nexus-3.86.2-01
    - name: "Extract expected directory name from filename"
      ansible.builtin.set_fact:
        # Removes .tar.gz and -unix/-linux suffixes to get the folder name
        extracted_dir_name: "{{ (nexus_tarball | basename) | regex_replace('(-unix|-linux-x86_64)?\\.tar\\.gz$', '') }}"

    - name: "Set full path for the new release"
      ansible.builtin.set_fact:
        new_nexus_dir: "{{ nexus_root }}/{{ extracted_dir_name }}"

    # 3. Extract the file
    # Note: Nexus Repo tarballs usually contain the folder structure inside them
    - name: "Extract Nexus tarball"
      ansible.builtin.unarchive:
        src: "{{ nexus_tarball }}"
        dest: "{{ nexus_root }}"
        remote_src: yes
        creates: "{{ new_nexus_dir }}"
