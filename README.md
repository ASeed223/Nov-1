- name: Stop Nexus HA 01 on lxpd208
  hosts: lxpd208
  gather_facts: no
  any_errors_fatal: true
  tasks:
    - name: Stop Nexus HA 01
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus stop
      register: stop_output
      # Do not fail if the service is already stopped (PID file missing)
      failed_when: 
        - stop_output.rc != 0 
        - '"PID file not found" not in stop_output.stdout'
        - '"not running" not in stop_output.stdout'
      changed_when: stop_output.rc == 0

    - name: Wait until Nexus HA 01 is stopped
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus status
      register: status_check
      # Status command returns non-zero when stopped, so we must ignore errors here
      failed_when: false
      changed_when: false
      retries: 12
      delay: 5
      # Check for multiple conditions indicating the service is down
      until: >
        status_check.rc != 0 or
        'stopped' in status_check.stdout.lower() or 
        'not running' in status_check.stdout.lower()

    - name: Fail if Nexus HA 01 is still running
      ansible.builtin.fail:
        msg: "Nexus HA 01 is still running on lxpd208!"
      # Double check that we only fail if it is explicitly running
      when: 
        - status_check.rc == 0
        - '"running" in status_check.stdout.lower()'
