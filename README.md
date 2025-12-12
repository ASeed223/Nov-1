- name: Stop Nexus HA 01 on lxpd208 (Process Based)
  hosts: lxpd208
  gather_facts: no
  any_errors_fatal: true
  tasks:
    - name: Check if Nexus is currently running (Process check)
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: initial_process_check
      # grep returns 0 if process exists (Running), 1 if not found (Stopped)
      failed_when: false
      changed_when: false

    - name: Stop Nexus HA 01 (Only if running)
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus stop
      register: stop_result
      # Only run this task if the initial check found the process (rc == 0)
      when: initial_process_check.rc == 0
      # Handle potential "PID file not found" error gracefully
      failed_when: 
        - stop_result.rc != 0 
        - '"PID file not found" not in stop_result.stdout'
      changed_when: stop_result.rc == 0

    - name: Verify Nexus is completely stopped (Retry for 1 minute)
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: verify_stop
      # We want grep to FAIL (rc != 0), which means no process was found.
      # If grep succeeds (rc == 0), it means process is still there, so we retry.
      until: verify_stop.rc != 0
      retries: 12
      delay: 5
      changed_when: false
      # Important: Ignore errors here so the loop doesn't crash the playbook immediately.
      # We want the next task to handle the failure message.
      ignore_errors: true

    - name: Fail if Nexus HA 01 is still running
      ansible.builtin.fail:
        msg: "Nexus HA 01 is still running on lxpd208!"
      # Fail if the previous verify task still found the process (rc == 0)
      when: verify_stop.rc == 0
