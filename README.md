The HTTP 502 (Bad Gateway) error was caused by Maven Central updating its SSL certificate on December 6, 2025. Since the new certificate was not trusted by the Nexus truststore, the connection failed with an SSLHandshakeException (PKIX path building failed). As a result, Nexus was unable to download any dependencies that were not already cached locally.

To resolve this, I manually imported the updated SSL certificate into the Nexus truststore, which successfully brought the repository back to Online – Ready to Connect.

This fix resolved the issue for the majority of the repositories. However, the RedHatMaven repository is still experiencing problems. I will need to spend more time investigating whether this repository can be fixed as well.
