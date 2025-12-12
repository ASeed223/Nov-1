- name: Stop Nexus HA 01 on lxpd208 (Process Based)
  hosts: lxpd208
  gather_facts: no
  any_errors_fatal: true
  tasks:
    - name: Check if Nexus is currently running (Process check)
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: initial_process_check
      # grep returns 0 if process exists, 1 if not found. We don't want to fail here.
      failed_when: false
      changed_when: false

    - name: Stop Nexus HA 01 (Only if running)
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus stop
      register: stop_result
      # Only run if the initial check found the process
      when: initial_process_check.rc == 0
      failed_when: 
        - stop_result.rc != 0 
        - '"PID file not found" not in stop_result.stdout'
      changed_when: stop_result.rc == 0

    - name: Verify Nexus is completely stopped (Retry for 1 minute)
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: verify_stop
      # Loop until rc is NOT 0 (meaning grep failed to find the process, so it is stopped)
      until: verify_stop.rc != 0
      retries: 12
      delay: 5
      changed_when: false
      # KEY FIX: Use failed_when: false instead of ignore_errors.
      # This prevents the red "fatal" error when grep returns 1 (not found).
      failed_when: false

    - name: Fail if Nexus HA 01 is still running
      ansible.builtin.fail:
        msg: "Nexus HA 01 is still running on lxpd208!"
      # If verify_stop.rc is still 0, it means grep still found the process
      when: verify_stop.rc == 0
