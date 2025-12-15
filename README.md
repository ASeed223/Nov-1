- name: Start Nexus HA 02 on lxpd209
  hosts: lxpd209
  gather_facts: no
  any_errors_fatal: true
  tasks:
    - name: Check if Nexus is currently running
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: initial_process_check
      # grep returns 0 if process exists, 1 if not found.
      failed_when: false
      changed_when: false

    - name: Start Nexus HA 02 (Only if NOT running)
      ansible.builtin.shell: /opt/nexus/nexus/bin/nexus start
      register: start_result
      # Only run this task if the initial check DID NOT find the process (rc != 0)
      when: initial_process_check.rc != 0
      failed_when: start_result.rc != 0
      changed_when: start_result.rc == 0

    - name: Verify Nexus is running (Retry for 1 minute)
      ansible.builtin.shell: ps -ef | grep java | grep "/opt/nexus/nexus" | grep -v grep
      register: verify_start
      until: verify_start.rc == 0
      retries: 12
      delay: 5
      changed_when: false
      # Prevent failure during the retry loop if process hasn't appeared yet
      failed_when: false

    - name: Fail if Nexus HA 02 failed to start
      ansible.builtin.fail:
        msg: "Nexus HA 02 failed to start on lxpd209 (Process not found)!"
      # Fail if the verify task returned anything other than 0 (meaning grep failed to find it)
      when: verify_start.rc != 0
