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
