vi /opt/nexus/sonatype-work/nexus3/etc/nexus.properties

This master password is used to encrypt/decrypt sensitive data (proxy passwords, LDAP bind, etc.) in the Nexus database.

Important for HA: This key must be identical on both lxpd208 and lxpd209. If updated, the physical master.key file in /opt/nexus/sonatype-work/nexus3/security/ must be synchronized between nodes to ensure successful failover.
