[cmdeploy@lxpd208 ~]$ /opt/nexus/nexus/bin/nexus run
2025-12-10 15:31:26,015-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.configuration.NexusProperties - nexus.properties: {ssl.etc=/opt/nexus/sonatype-work/nexus3/etc/ssl, nexus-edition=nexus-pro-edition, java.specification.version=17, nexus-db-feature=nexus-datastore-mybatis, sun.jnu.encoding=UTF-8, nexus.view.exhaustForAgents=Apache-Maven.*|libwww-perl.*, sun.arch.data.model=64, java.vendor.url=https://adoptium.net/, nexus.session.enabled=false, nexus.scripts.allowCreation=true, sun.boot.library.path=/opt/nexus/nexus-3.86.2-01/jdk/temurin_17.0.13_11_linux_x86_64/jdk-17.0.13+11/lib, sun.java.command=/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar, logging.register-shutdown-hook=false, jdk.debug=release, sun.stderr.encoding=UTF-8, java.specification.vendor=Oracle Corporation, java.version.date=2024-10-15, java.home=/opt/nexus/nexus-3.86.2-01/jdk/temurin_17.0.13_11_linux_x86_64/jdk-17.0.13+11, logging.config=etc/logback/logback.xml, nexus-features=nexus-pro-feature, file.separator=/, java.vm.compressedOopsMode=Zero based, line.separator=
, sun.stdout.encoding=UTF-8, nexus.onboarding.enabled=true, java.vm.specification.vendor=Oracle Corporation, java.specification.name=Java Platform API Specification, spring.config.location=etc/default-application.properties, application-host=0.0.0.0, jdk.tls.ephemeralDHKeySize=2048, nexus-context-path=/, java.util.logging.config.file=etc/spring/java.util.logging.properties, java.protocol.handler.pkgs=org.springframework.boot.loader.net.protocol, sun.management.compiler=HotSpot 64-Bit Tiered Compilers, karaf.home=., java.runtime.version=17.0.13+11, user.name=cmdeploy, nexus.jwt.enabled=true, nexus.datastore.clustered.enabled=true, file.encoding=UTF-8, java.vendor.version=Temurin-17.0.13+11, java.io.tmpdir=/opt/nexus/sonatype-work/nexus3/tmp, logback.etc=/opt/nexus/nexus-3.86.2-01/etc/logback, java.version=17.0.13, fabric.etc=/opt/nexus/nexus-3.86.2-01/etc/fabric, java.vm.specification.name=Java Virtual Machine Specification, PID=1713832, nexus.change.repo.blobstore.task.enabled=true, CONSOLE_LOG_CHARSET=UTF-8, native.encoding=UTF-8, java.library.path=/opt/CA/DSM/caf/lib:/opt/CA/SharedComponents/lib:/usr/java/packages/lib:/usr/lib64:/lib64:/lib:/usr/lib, java.vendor=Eclipse Adoptium, java.specification.maintenance.version=1, karaf.base=/opt/nexus/nexus-3.86.2-01, sun.io.unicode.encoding=UnicodeLittle, karaf.log=/opt/nexus/sonatype-work/nexus3/log, karaf.startLocalConsole=false, java.class.path=/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar, karaf.etc=/opt/nexus/nexus-3.86.2-01/etc/karaf, nexus.assetdownloads.enabled=true, java.vm.vendor=Eclipse Adoptium, nexus.installer.type=linux-x86-64, user.timezone=America/Los_Angeles, org.jboss.logging.provider=slf4j, application-port=8081, java.vm.specification.version=17, os.name=Linux, sun.java.launcher=SUN_STANDARD, user.country=US, karaf.data=/opt/nexus/sonatype-work/nexus3, nexus.licenseFile=/home/cmdeploy/license/a617d2decad9bce4fbd4f955ba2d10e86298c7c7.lic, karaf.instances=/opt/nexus/sonatype-work/nexus3/instances, sun.cpu.endian=little, user.home=/home/cmdeploy, user.language=en, nexus.elasticsearch.enabled=false, jetty.etc=/opt/nexus/nexus-3.86.2-01/etc/jetty, FILE_LOG_CHARSET=UTF-8, java.awt.headless=true, nexus.datastore.sql.cache.enabled=true, nexus.http.denyframe.enabled=true, java.net.preferIPv4Stack=true, nexus.datastore.enabled=true, path.separator=:, os.version=5.14.0-570.60.1.el9_6.x86_64, java.runtime.name=OpenJDK Runtime Environment, nexus-args=/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty.xml,/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml,/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-requestlog.xml, nexus.quartz.jobstore.jdbc=true, java.vm.name=OpenJDK 64-Bit Server VM, nexus.datastore.blobstore.metrics.enabled=true, java.vendor.url.bug=https://github.com/adoptium/adoptium-support/issues, org.sonatype.nexus.repository.httpbridge.internal.HttpBridgeModule.legacy=true, user.dir=/opt/nexus/nexus-3.86.2-01, os.arch=amd64, nexus.datastore.table.search.enabled=true, java.vm.info=mixed mode, sharing, java.vm.version=17.0.13+11, application-port-ssl=8443, java.class.version=61.0}
2025-12-10 15:31:26,023-0800 INFO  [main] *SYSTEM com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication - Starting SonatypeNexusRepositoryApplication v3.86.2-01 using Java 17.0.13 with PID 1713832 (/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar started by cmdeploy in /opt/nexus/nexus-3.86.2-01)
2025-12-10 15:31:26,024-0800 INFO  [main] *SYSTEM com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication - No active profile set, falling back to 1 default profile: "default"
2025-12-10 15:31:27,719-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.ApplicationLauncher - Starting nexus with edition PRO
2025-12-10 15:31:27,952-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.SpringComponentScan - Scanning for components in packages: [org.sonatype.nexus, com.sonatype.nexus]
2025-12-10 15:31:38,537-0800 INFO  [main] *SYSTEM org.sonatype.nexus.quartz.internal.QuartzSchedulerProvider - Thread-pool size: 20, Thread-pool priority: 5
2025-12-10 15:31:39,073-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.log.overrides.datastore.DatastoreLoggerOverrides - File: /opt/nexus/sonatype-work/nexus3/etc/logback/logback-overrides.xml
2025-12-10 15:31:39,076-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.log.overrides.file.LogbackLoggerOverrides - File: /opt/nexus/sonatype-work/nexus3/etc/logback/logback-overrides.xml
2025-12-10 15:31:39,112-0800 INFO  [main] *SYSTEM org.apache.shiro.nexus.NexusWebSessionManager - Global session timeout: 1800000 ms
2025-12-10 15:31:39,113-0800 INFO  [main] *SYSTEM org.apache.shiro.nexus.NexusWebSessionManager - Session-cookie prototype: name=NXSESSIONID, secure=true
2025-12-10 15:31:40,059-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle - UI plugin descriptors:
2025-12-10 15:31:40,059-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rapture
2025-12-10 15:31:40,059-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-coreui-plugin
2025-12-10 15:31:40,059-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle - ExtJS UI plugin descriptors:
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rapture
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rutauth-plugin
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-proximanova-plugin
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-coreui-plugin
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-proui-plugin
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-cargo
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-composer
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-onboarding-plugin
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-maven
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-docker
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-rubygems
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-npm
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-nuget
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-pypi
2025-12-10 15:31:40,060-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-saml-plugin
2025-12-10 15:31:40,061-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-analytics-plugin
2025-12-10 15:31:40,080-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.webresources.WebResourceServlet - Max-age: 30 days (2592000 seconds)
2025-12-10 15:31:40,089-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.wonderland.DownloadServiceImpl - Downloads directory: /opt/nexus/sonatype-work/nexus3/downloads
2025-12-10 15:31:40,268-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.atlas.SupportZipGeneratorImpl - Maximum included file size: 30 megabytes
2025-12-10 15:31:40,268-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.atlas.SupportZipGeneratorImpl - Maximum ZIP file size: 50 megabytes
2025-12-10 15:31:40,657-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Detected 1 engine-factories
2025-12-10 15:31:40,659-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Engine-factory: Groovy Scripting Engine v2.0; language=Groovy, version=3.0.19, names=[groovy, Groovy], mime-types=[application/x-groovy], extensions=[groovy]
2025-12-10 15:31:40,659-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Default language: groovy
2025-12-10 15:31:40,983-0800 INFO  [main] *SYSTEM org.hibernate.validator.internal.util.Version - HV000001: Hibernate Validator 6.2.0.Final
2025-12-10 15:31:42,261-0800 INFO  [main] *SYSTEM org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor - Inconsistent constructor declaration on bean with name 'maliciousRiskOnDiskAnalytics': single autowire-marked constructor flagged as optional - this constructor is effectively required since there is no default constructor to fall back to: public com.sonatype.analytics.internal.MaliciousRiskOnDiskAnalytics(com.sonatype.nexus.risk.visualizer.MaliciousRiskService,java.lang.Boolean)
2025-12-10 15:31:42,474-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Starting jetty
2025-12-10 15:31:42,486-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Applying configuration: file:/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty.xml
2025-12-10 15:31:42,839-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Applying configuration: file:/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml
2025-12-10 15:31:42,897-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Applying configuration: file:/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-requestlog.xml
2025-12-10 15:31:42,951-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Starting: oejs.Server@5274d11e{STOPPED}[12.0.17,sto=5000]
2025-12-10 15:31:42,958-0800 INFO  [jetty-main-1] *SYSTEM org.eclipse.jetty.server.Server - jetty-12.0.17; built: 2025-03-03T13:15:05.903Z; git: 14d19c268e4cb09afc312b5255a4cbb7a95c5cb6; jvm 17.0.13+11
2025-12-10 15:31:43,253-0800 INFO  [jetty-main-1] *SYSTEM org.eclipse.jetty.session.DefaultSessionIdManager - Session workerName=node0
2025-12-10 15:31:43,281-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.internal.NexusServletContextListener - Running lifecycle phases [KERNEL, STORAGE, RESTORE, UPGRADE, SCHEMAS, EVENTS, SECURITY, SERVICES, REPOSITORIES, CAPABILITIES, TASKS]
2025-12-10 15:31:43,377-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Indexing lifecycle managed components up to phase TASKS
2025-12-10 15:31:43,378-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Start KERNEL
2025-12-10 15:31:43,382-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.internal.log.LogbackLogManager - Configuring
2025-12-10 15:31:43,387-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Start STORAGE
2025-12-10 15:31:43,402-0800 INFO  [jetty-main-1] *SYSTEM com.sonatype.nexus.self.hosted.datastore.DataStoreConfigurationFileSource - Loaded 'nexus' data store configuration from properties file (postgresql)
2025-12-10 15:31:43,444-0800 INFO  [jetty-main-1] *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Starting...
2025-12-10 15:31:43,601-0800 INFO  [jetty-main-1] *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Start completed.
2025-12-10 15:31:43,603-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Loading MyBatis configuration from /opt/nexus/nexus-3.86.2-01/etc/fabric/mybatis.xml
2025-12-10 15:31:43,759-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - MyBatis databaseId: PostgreSQL
2025-12-10 15:31:43,979-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for JwtSecretDAO
2025-12-10 15:31:44,072-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for LoggingOverridesDAO
2025-12-10 15:31:44,094-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DeploymentIdDAO
2025-12-10 15:31:44,111-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NodeIdDAO
2025-12-10 15:31:44,133-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AnonymousConfigurationDAO
2025-12-10 15:31:44,165-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CPrivilegeDAO
2025-12-10 15:31:44,190-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CRoleDAO
2025-12-10 15:31:44,213-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CUserRoleMappingDAO
2025-12-10 15:31:44,228-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CUserDAO
2025-12-10 15:31:44,238-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RealmConfigurationDAO
2025-12-10 15:31:44,251-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SecretsDAO
2025-12-10 15:31:44,263-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SoftDeletedBlobsDAO
2025-12-10 15:31:44,277-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CleanupPolicyDAO
2025-12-10 15:31:44,292-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CapabilityStorageItemDAO
2025-12-10 15:31:44,305-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for EmailConfigurationDAO
2025-12-10 15:31:44,316-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HttpClientConfigurationDAO
2025-12-10 15:31:44,331-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ApiKeyDAO
2025-12-10 15:31:44,346-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ApiKeyV2DAO
2025-12-10 15:31:44,359-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SelectorConfigurationDAO
2025-12-10 15:31:44,371-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NexusKeyValueDAO
2025-12-10 15:31:44,382-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for QuartzDAO
2025-12-10 15:31:44,397-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConfigurationDAO
2025-12-10 15:31:44,411-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for BlobStoreConfigurationDAO
2025-12-10 15:31:44,423-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RoutingRuleDAO
2025-12-10 15:31:44,433-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for BlobStoreMetricsDAO
2025-12-10 15:31:44,446-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for UpgradeTaskDAO
2025-12-10 15:31:44,459-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ScriptDAO
2025-12-10 15:31:44,471-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for LdapConfigurationDAO
2025-12-10 15:31:44,481-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for KeyStoreDAO
2025-12-10 15:31:44,491-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for TrustedSSLCertificateDAO
2025-12-10 15:31:44,512-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComponentApplicationScanScheduleDAO
2025-12-10 15:31:44,524-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComponentApplicationScanDAO
2025-12-10 15:31:44,537-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ReconcilePlanDetailsDAO
2025-12-10 15:31:44,561-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ReconcilePlanDAO
2025-12-10 15:31:44,582-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CooperationDAO
2025-12-10 15:31:44,592-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DistributedEventDAO
2025-12-10 15:31:44,601-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ClockDAO
2025-12-10 15:31:44,609-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for FreezeRequestDAO
2025-12-10 15:31:44,637-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SearchTableDAO
2025-12-10 15:31:44,657-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CacheDAO
2025-12-10 15:31:44,670-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SupportZipInfoDAO
2025-12-10 15:31:44,680-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DistributedAuthTicketCacheDAO
2025-12-10 15:31:44,690-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for FirewallIgnorePatternsDAO
2025-12-10 15:31:44,700-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RepositoryHealthCheckConfigurationDAO
2025-12-10 15:31:44,710-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for MalwareRemediatorTaskDAO
2025-12-10 15:31:44,727-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RepositoryMetricsDAO
2025-12-10 15:31:44,743-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NodeHeartbeatDAO
2025-12-10 15:31:44,762-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ChangeRepositoryBlobstoreDAO
2025-12-10 15:31:44,774-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SamlConfigurationDAO
2025-12-10 15:31:44,785-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for SamlUserDAO
2025-12-10 15:31:44,798-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for TagDAO
2025-12-10 15:31:44,809-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for UserTokenRecordDAO
2025-12-10 15:31:44,820-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AggregatedMetricsDAO
2025-12-10 15:31:44,833-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for MetricDAO
2025-12-10 15:31:44,852-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptContentRepositoryDAO
2025-12-10 15:31:44,867-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptAssetBlobDAO
2025-12-10 15:31:44,903-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptComponentDAO
2025-12-10 15:31:44,949-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptAssetDAO
2025-12-10 15:31:44,964-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptBrowseNodeDAO
2025-12-10 15:31:44,977-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptKeyValueDAO
2025-12-10 15:31:44,988-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2ContentRepositoryDAO
2025-12-10 15:31:45,001-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2AssetBlobDAO
2025-12-10 15:31:45,027-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2ComponentDAO
2025-12-10 15:31:45,057-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2AssetDAO
2025-12-10 15:31:45,072-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2BrowseNodeDAO
2025-12-10 15:31:45,084-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawContentRepositoryDAO
2025-12-10 15:31:45,098-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawAssetBlobDAO
2025-12-10 15:31:45,116-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawComponentDAO
2025-12-10 15:31:45,136-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawAssetDAO
2025-12-10 15:31:45,150-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawBrowseNodeDAO
2025-12-10 15:31:45,160-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoContentRepositoryDAO
2025-12-10 15:31:45,172-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoAssetBlobDAO
2025-12-10 15:31:45,189-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoComponentDAO
2025-12-10 15:31:45,208-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoAssetDAO
2025-12-10 15:31:45,221-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoBrowseNodeDAO
2025-12-10 15:31:45,232-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsContentRepositoryDAO
2025-12-10 15:31:45,244-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsAssetBlobDAO
2025-12-10 15:31:45,260-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsComponentDAO
2025-12-10 15:31:45,280-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsAssetDAO
2025-12-10 15:31:45,295-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsBrowseNodeDAO
2025-12-10 15:31:45,305-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerContentRepositoryDAO
2025-12-10 15:31:45,317-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerAssetBlobDAO
2025-12-10 15:31:45,378-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerComponentDAO
2025-12-10 15:31:45,400-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerAssetDAO
2025-12-10 15:31:45,413-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerBrowseNodeDAO
2025-12-10 15:31:45,423-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanContentRepositoryDAO
2025-12-10 15:31:45,434-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanAssetBlobDAO
2025-12-10 15:31:45,451-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanComponentDAO
2025-12-10 15:31:45,470-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanAssetDAO
2025-12-10 15:31:45,483-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanBrowseNodeDAO
2025-12-10 15:31:45,494-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaContentRepositoryDAO
2025-12-10 15:31:45,507-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaAssetBlobDAO
2025-12-10 15:31:45,523-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaComponentDAO
2025-12-10 15:31:45,542-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaAssetDAO
2025-12-10 15:31:45,555-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaBrowseNodeDAO
2025-12-10 15:31:45,565-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerContentRepositoryDAO
2025-12-10 15:31:45,578-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerAssetBlobDAO
2025-12-10 15:31:45,594-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerComponentDAO
2025-12-10 15:31:45,613-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerAssetDAO
2025-12-10 15:31:45,625-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerBrowseNodeDAO
2025-12-10 15:31:45,635-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerForeignLayersDAO
2025-12-10 15:31:45,645-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsContentRepositoryDAO
2025-12-10 15:31:45,657-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsAssetBlobDAO
2025-12-10 15:31:45,673-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsComponentDAO
2025-12-10 15:31:45,692-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsAssetDAO
2025-12-10 15:31:45,706-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsBrowseNodeDAO
2025-12-10 15:31:45,716-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoContentRepositoryDAO
2025-12-10 15:31:45,728-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoAssetBlobDAO
2025-12-10 15:31:45,750-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoComponentDAO
2025-12-10 15:31:45,776-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoAssetDAO
2025-12-10 15:31:45,793-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoBrowseNodeDAO
2025-12-10 15:31:45,803-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmContentRepositoryDAO
2025-12-10 15:31:45,817-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmAssetBlobDAO
2025-12-10 15:31:45,838-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmComponentDAO
2025-12-10 15:31:45,862-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmAssetDAO
2025-12-10 15:31:45,879-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmBrowseNodeDAO
2025-12-10 15:31:45,889-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmKeyValueDAO
2025-12-10 15:31:45,899-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceContentRepositoryDAO
2025-12-10 15:31:45,911-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceAssetBlobDAO
2025-12-10 15:31:45,926-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceComponentDAO
2025-12-10 15:31:45,943-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceAssetDAO
2025-12-10 15:31:45,956-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceBrowseNodeDAO
2025-12-10 15:31:45,965-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmContentRepositoryDAO
2025-12-10 15:31:45,976-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmAssetBlobDAO
2025-12-10 15:31:45,991-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmComponentDAO
2025-12-10 15:31:46,008-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmAssetDAO
2025-12-10 15:31:46,020-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmBrowseNodeDAO
2025-12-10 15:31:46,031-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetContentRepositoryDAO
2025-12-10 15:31:46,041-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetAssetBlobDAO
2025-12-10 15:31:46,057-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetComponentDAO
2025-12-10 15:31:46,075-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetAssetDAO
2025-12-10 15:31:46,087-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetBrowseNodeDAO
2025-12-10 15:31:46,097-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2ContentRepositoryDAO
2025-12-10 15:31:46,107-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2AssetBlobDAO
2025-12-10 15:31:46,122-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2ComponentDAO
2025-12-10 15:31:46,139-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2AssetDAO
2025-12-10 15:31:46,151-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2BrowseNodeDAO
2025-12-10 15:31:46,161-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiContentRepositoryDAO
2025-12-10 15:31:46,172-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiAssetBlobDAO
2025-12-10 15:31:46,187-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiComponentDAO
2025-12-10 15:31:46,205-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiAssetDAO
2025-12-10 15:31:46,217-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiBrowseNodeDAO
2025-12-10 15:31:46,226-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RContentRepositoryDAO
2025-12-10 15:31:46,236-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RAssetBlobDAO
2025-12-10 15:31:46,251-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RComponentDAO
2025-12-10 15:31:46,268-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RAssetDAO
2025-12-10 15:31:46,280-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RBrowseNodeDAO
2025-12-10 15:31:46,290-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsContentRepositoryDAO
2025-12-10 15:31:46,301-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsAssetBlobDAO
2025-12-10 15:31:46,316-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsComponentDAO
2025-12-10 15:31:46,335-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsAssetDAO
2025-12-10 15:31:46,347-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsBrowseNodeDAO
2025-12-10 15:31:46,357-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumContentRepositoryDAO
2025-12-10 15:31:46,368-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumAssetBlobDAO
2025-12-10 15:31:46,383-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumComponentDAO
2025-12-10 15:31:46,401-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumAssetDAO
2025-12-10 15:31:46,413-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumBrowseNodeDAO
2025-12-10 15:31:46,424-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumKeyValueDAO
2025-12-10 15:31:46,434-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for AptComponentTagDAO
2025-12-10 15:31:46,443-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CargoComponentTagDAO
2025-12-10 15:31:46,453-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CocoapodsComponentTagDAO
2025-12-10 15:31:46,463-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ComposerComponentTagDAO
2025-12-10 15:31:46,472-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for ConanComponentTagDAO
2025-12-10 15:31:46,481-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for CondaComponentTagDAO
2025-12-10 15:31:46,491-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for DockerComponentTagDAO
2025-12-10 15:31:46,500-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GitLfsComponentTagDAO
2025-12-10 15:31:46,509-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for GoComponentTagDAO
2025-12-10 15:31:46,518-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HelmComponentTagDAO
2025-12-10 15:31:46,527-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for HuggingFaceComponentTagDAO
2025-12-10 15:31:46,537-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for Maven2ComponentTagDAO
2025-12-10 15:31:46,546-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NpmComponentTagDAO
2025-12-10 15:31:46,555-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for NugetComponentTagDAO
2025-12-10 15:31:46,564-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for P2ComponentTagDAO
2025-12-10 15:31:46,574-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for PypiComponentTagDAO
2025-12-10 15:31:46,583-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RComponentTagDAO
2025-12-10 15:31:46,593-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RawComponentTagDAO
2025-12-10 15:31:46,602-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for RubygemsComponentTagDAO
2025-12-10 15:31:46,610-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.datastore.mybatis.MyBatisDataStore - nexus - Creating schema for YumComponentTagDAO
2025-12-10 15:31:46,988-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Start RESTORE
2025-12-10 15:31:46,989-0800 INFO  [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Start UPGRADE
2025-12-10 15:31:47,187-0800 ERROR [jetty-main-1] *SYSTEM com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator - unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
2025-12-10 15:31:47,188-0800 ERROR [jetty-main-1] *SYSTEM org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl - Failed transition: NEW -> STARTED
java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
2025-12-10 15:31:47,195-0800 ERROR [jetty-main-1] *SYSTEM org.sonatype.nexus.extender.internal.NexusServletContextListener - Failed to initialize context
java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
2025-12-10 15:31:47,200-0800 WARN  [jetty-main-1] *SYSTEM org.eclipse.jetty.ee8.webapp.WebAppContext - Failed startup of context oeje8w.WebAppContext@61c4c9bc{Sonatype Nexus,/,null,false}
java.lang.RuntimeException: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:73)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
Caused by: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        ... 33 common frames omitted
2025-12-10 15:31:47,211-0800 ERROR [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Start failed
java.lang.RuntimeException: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:73)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
Caused by: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        ... 33 common frames omitted
2025-12-10 15:31:47,211-0800 ERROR [jetty-main-1] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Failed to start
java.lang.RuntimeException: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:73)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
Caused by: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        ... 33 common frames omitted
2025-12-10 15:31:47,216-0800 WARN  [main] *SYSTEM org.springframework.context.annotation.AnnotationConfigApplicationContext - Exception encountered during context initialization - cancelling refresh attempt: org.springframework.context.ApplicationContextException: Failed to start bean 'org.sonatype.nexus.bootstrap.jetty.ManagedJetty'
2025-12-10 15:31:47,225-0800 WARN  [JettyShutdownThread] *SYSTEM org.eclipse.jetty.util.component.ContainerLifeCycle - Unable to destroy
java.lang.IllegalStateException: !STOPPED
        at org.eclipse.jetty.ee8.nested.HandlerWrapper.destroy(HandlerWrapper.java:119)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.destroy(WebAppContext.java:548)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.destroy(ContainerLifeCycle.java:228)
        at org.eclipse.jetty.server.Handler$Abstract.destroy(Handler.java:507)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$destroy$2(ContextHandler.java:1018)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.run(ContextHandler.java:1517)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.run(ContextHandler.java:1504)
        at org.eclipse.jetty.server.handler.ContextHandler.destroy(ContextHandler.java:1018)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.destroy(ContainerLifeCycle.java:228)
        at org.eclipse.jetty.server.Handler$Abstract.destroy(Handler.java:507)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.destroy(ContainerLifeCycle.java:228)
        at org.eclipse.jetty.server.Handler$Abstract.destroy(Handler.java:507)
        at org.eclipse.jetty.util.thread.ShutdownThread.run(ShutdownThread.java:142)
2025-12-10 15:31:47,294-0800 WARN  [main] *SYSTEM org.springframework.context.annotation.AnnotationConfigApplicationContext - Exception encountered during context initialization - cancelling refresh attempt: java.lang.RuntimeException: Failed to configure application
2025-12-10 15:31:47,295-0800 ERROR [main] *SYSTEM org.springframework.boot.SpringApplication - Application run failed
java.lang.RuntimeException: Failed to configure application
        at org.sonatype.nexus.bootstrap.entrypoint.ApplicationLauncher.onContextRefreshed(ApplicationLauncher.java:95)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:569)
        at org.springframework.context.event.ApplicationListenerMethodAdapter.doInvoke(ApplicationListenerMethodAdapter.java:383)
        at org.springframework.context.event.ApplicationListenerMethodAdapter.processEvent(ApplicationListenerMethodAdapter.java:255)
        at org.springframework.context.event.ApplicationListenerMethodAdapter.onApplicationEvent(ApplicationListenerMethodAdapter.java:174)
        at org.springframework.context.event.SimpleApplicationEventMulticaster.doInvokeListener(SimpleApplicationEventMulticaster.java:185)
        at org.springframework.context.event.SimpleApplicationEventMulticaster.invokeListener(SimpleApplicationEventMulticaster.java:178)
        at org.springframework.context.event.SimpleApplicationEventMulticaster.multicastEvent(SimpleApplicationEventMulticaster.java:156)
        at org.springframework.context.support.AbstractApplicationContext.publishEvent(AbstractApplicationContext.java:454)
        at org.springframework.context.support.AbstractApplicationContext.publishEvent(AbstractApplicationContext.java:387)
        at org.springframework.context.support.AbstractApplicationContext.finishRefresh(AbstractApplicationContext.java:1009)
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:630)
        at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:754)
        at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:456)
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:335)
        at org.springframework.boot.builder.SpringApplicationBuilder.run(SpringApplicationBuilder.java:149)
        at com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication.main(SonatypeNexusRepositoryApplication.java:48)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:569)
        at org.springframework.boot.loader.launch.Launcher.launch(Launcher.java:102)
        at org.springframework.boot.loader.launch.Launcher.launch(Launcher.java:64)
        at org.springframework.boot.loader.launch.JarLauncher.main(JarLauncher.java:40)
Caused by: org.springframework.context.ApplicationContextException: Failed to start bean 'org.sonatype.nexus.bootstrap.jetty.ManagedJetty'
        at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:408)
        at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:394)
        at org.springframework.context.support.DefaultLifecycleProcessor$LifecycleGroup.start(DefaultLifecycleProcessor.java:586)
        at java.base/java.lang.Iterable.forEach(Iterable.java:75)
        at org.springframework.context.support.DefaultLifecycleProcessor.startBeans(DefaultLifecycleProcessor.java:364)
        at org.springframework.context.support.DefaultLifecycleProcessor.onRefresh(DefaultLifecycleProcessor.java:310)
        at org.springframework.context.support.AbstractApplicationContext.finishRefresh(AbstractApplicationContext.java:1006)
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:630)
        at org.sonatype.nexus.bootstrap.entrypoint.SpringComponentScan.finishBootstrapComponentScanning(SpringComponentScan.java:90)
        at org.sonatype.nexus.bootstrap.entrypoint.ApplicationLauncher.onContextRefreshed(ApplicationLauncher.java:92)
        ... 26 common frames omitted
Caused by: java.lang.RuntimeException: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:73)
        at org.eclipse.jetty.ee8.nested.ContextHandler.callContextInitialized(ContextHandler.java:786)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.callContextInitialized(ServletContextHandler.java:516)
        at org.eclipse.jetty.ee8.nested.ContextHandler.contextInitialized(ContextHandler.java:735)
        at org.eclipse.jetty.ee8.servlet.ServletHandler.initialize(ServletHandler.java:629)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.startContext(ServletContextHandler.java:311)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startWebapp(WebAppContext.java:1195)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.startContext(WebAppContext.java:1165)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStartInContext(ContextHandler.java:626)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1450)
        at org.eclipse.jetty.ee8.nested.ContextHandler.doStart(ContextHandler.java:615)
        at org.eclipse.jetty.ee8.servlet.ServletContextHandler.doStart(ServletContextHandler.java:243)
        at org.eclipse.jetty.ee8.webapp.WebAppContext.doStart(WebAppContext.java:502)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:113)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.handler.ContextHandler.lambda$doStart$0(ContextHandler.java:757)
        at org.eclipse.jetty.server.handler.ContextHandler$ScopedContext.call(ContextHandler.java:1456)
        at org.eclipse.jetty.server.handler.ContextHandler.doStart(ContextHandler.java:757)
        at org.eclipse.jetty.ee8.nested.ContextHandler$CoreContextHandler.doStart(ContextHandler.java:2290)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at io.dropwizard.metrics.jetty12.AbstractInstrumentedHandler.doStart(AbstractInstrumentedHandler.java:149)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.start(ContainerLifeCycle.java:169)
        at org.eclipse.jetty.server.Server.start(Server.java:641)
        at org.eclipse.jetty.util.component.ContainerLifeCycle.doStart(ContainerLifeCycle.java:120)
        at org.eclipse.jetty.server.Handler$Abstract.doStart(Handler.java:491)
        at org.eclipse.jetty.server.Server.doStart(Server.java:582)
        at org.eclipse.jetty.util.component.AbstractLifeCycle.start(AbstractLifeCycle.java:93)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer$JettyMainThread.run(JettyServer.java:374)
Caused by: java.lang.IllegalStateException: unable to perform clustered deployment for node 902c3509-2759-4287-a0b2-534fb6c1308f , found inconsistencies :
There are other Nexus Repository instance(s) that are currently running in this HA cluster with a different version. Please stop these instances.
Node ID: fc8152a5-bbff-41cb-8068-269dfb76eae0 Version: 3.75.0-06
Node ID: 3a0f7b81-8885-46b3-9dce-9b5edcc5be53 Version: 3.75.0-06
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.buildAndThrowError(ClusteredDeploymentValidator.java:161)
        at com.sonatype.nexus.self.hosted.distributed.ClusteredDeploymentValidator.validate(ClusteredDeploymentValidator.java:122)
        at java.base/java.util.Optional.ifPresent(Optional.java:178)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:70)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start_aroundBody0(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport$AjcClosure1.run(StateGuardLifecycleSupport.java:1)
        at org.aspectj.runtime.reflect.JoinPointImpl.proceed(JoinPointImpl.java:164)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.lambda$0(TransitionsAspect.java:57)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:217)
        at org.sonatype.nexus.common.stateguard.TransitionsAspect.aroundTransitionsMethod(TransitionsAspect.java:55)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:68)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:154)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:110)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.moveToPhase(NexusServletContextListener.java:113)
        at org.sonatype.nexus.extender.internal.NexusServletContextListener.contextInitialized(NexusServletContextListener.java:69)
        ... 33 common frames omitted
