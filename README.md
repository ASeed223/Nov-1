- name: "Ensure archive directory exists"
      ansible.builtin.file:
        path: "{{ nexus_root }}/archive"
        state: directory
        mode: '0755'

    - name: "Move tarball to archive folder"
      ansible.builtin.command:
        cmd: "mv {{ nexus_tarball }} {{ nexus_root }}/archive/"
      args:
        # Only runs if the file exists (prevents errors on re-run)
        removes: "{{ nexus_tarball }}"

    - name: "Display Archive Result"
      ansible.builtin.debug:
        msg: "Moved {{ nexus_tarball_name }} to {{ nexus_root }}/archive/"
