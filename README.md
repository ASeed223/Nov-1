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

    - name: Wait until Nexus HA 01 is stopped (Script Check)
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus status
      register: status_check
      # Status command returns non-zero when stopped, so we must ignore errors here
      failed_when: false
      changed_when: false
      retries: 24  # Increased to 2 minutes (5s * 24) for safe shutdown
      delay: 5
      # Check for multiple conditions indicating the service is down
      until: >
        status_check.rc != 0 or
        'stopped' in status_check.stdout.lower() or 
        'not running' in status_check.stdout.lower()

    - name: Verify process is gone (Kernel Check)
      # This is more accurate than the 'status' script.
      # It checks if any java process for Nexus is actually running.
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: process_check
      # 'grep' returns 1 if NO lines are found (which means success/stopped)
      # 'grep' returns 0 if lines ARE found (which means it is still running)
      failed_when: false
      changed_when: false

    - name: Fail if Nexus HA 01 is still running
      ansible.builtin.fail:
        msg: "Nexus HA 01 is still running on lxpd208 (Java Process Detected)!"
      # Fail if grep found a process (rc=0) OR if the script says it's running
      when: 
        - process_check.rc == 0
