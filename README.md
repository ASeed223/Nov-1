[cmdeploy@lxpd209 ~]$ /opt/nexus/nexus/bin/nexus run
2025-12-10 15:54:55,114-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.configuration.NexusProperties - nexus.properties: {ssl.etc=/opt/nexus/sonatype-work/nexus3/etc/ssl, nexus-edition=nexus-pro-edition, java.specification.version=17, nexus-db-feature=nexus-datastore-mybatis, sun.jnu.encoding=UTF-8, nexus.view.exhaustForAgents=Apache-Maven.*|libwww-perl.*, sun.arch.data.model=64, java.vendor.url=https://adoptium.net/, nexus.session.enabled=false, nexus.scripts.allowCreation=true, sun.boot.library.path=/opt/nexus/nexus-3.86.2-01/jdk/temurin_17.0.13_11_linux_x86_64/jdk-17.0.13+11/lib, sun.java.command=/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar, logging.register-shutdown-hook=false, jdk.debug=release, sun.stderr.encoding=UTF-8, java.specification.vendor=Oracle Corporation, java.version.date=2024-10-15, java.home=/opt/nexus/nexus-3.86.2-01/jdk/temurin_17.0.13_11_linux_x86_64/jdk-17.0.13+11, logging.config=etc/logback/logback.xml, nexus-features=nexus-pro-feature, file.separator=/, java.vm.compressedOopsMode=Zero based, line.separator=
, sun.stdout.encoding=UTF-8, nexus.onboarding.enabled=true, java.vm.specification.vendor=Oracle Corporation, java.specification.name=Java Platform API Specification, spring.config.location=etc/default-application.properties, application-host=0.0.0.0, jdk.tls.ephemeralDHKeySize=2048, nexus-context-path=/, java.util.logging.config.file=etc/spring/java.util.logging.properties, java.protocol.handler.pkgs=org.springframework.boot.loader.net.protocol, sun.management.compiler=HotSpot 64-Bit Tiered Compilers, karaf.home=., java.runtime.version=17.0.13+11, user.name=cmdeploy, nexus.jwt.enabled=true, nexus.datastore.clustered.enabled=true, file.encoding=UTF-8, java.vendor.version=Temurin-17.0.13+11, java.io.tmpdir=/opt/nexus/sonatype-work/nexus3/tmp, logback.etc=/opt/nexus/nexus-3.86.2-01/etc/logback, java.version=17.0.13, fabric.etc=/opt/nexus/nexus-3.86.2-01/etc/fabric, java.vm.specification.name=Java Virtual Machine Specification, PID=1853318, nexus.change.repo.blobstore.task.enabled=true, CONSOLE_LOG_CHARSET=UTF-8, native.encoding=UTF-8, java.library.path=/opt/CA/DSM/caf/lib:/opt/CA/SharedComponents/lib:/usr/java/packages/lib:/usr/lib64:/lib64:/lib:/usr/lib, java.vendor=Eclipse Adoptium, java.specification.maintenance.version=1, karaf.base=/opt/nexus/nexus-3.86.2-01, sun.io.unicode.encoding=UnicodeLittle, karaf.log=/opt/nexus/sonatype-work/nexus3/log, karaf.startLocalConsole=false, java.class.path=/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar, karaf.etc=/opt/nexus/nexus-3.86.2-01/etc/karaf, nexus.assetdownloads.enabled=true, java.vm.vendor=Eclipse Adoptium, nexus.installer.type=linux-x86-64, user.timezone=America/Los_Angeles, org.jboss.logging.provider=slf4j, application-port=8081, java.vm.specification.version=17, os.name=Linux, sun.java.launcher=SUN_STANDARD, user.country=US, karaf.data=/opt/nexus/sonatype-work/nexus3, nexus.licenseFile=/home/cmdeploy/license/a617d2decad9bce4fbd4f955ba2d10e86298c7c7.lic, karaf.instances=/opt/nexus/sonatype-work/nexus3/instances, sun.cpu.endian=little, user.home=/home/cmdeploy, user.language=en, nexus.elasticsearch.enabled=false, jetty.etc=/opt/nexus/nexus-3.86.2-01/etc/jetty, FILE_LOG_CHARSET=UTF-8, java.awt.headless=true, nexus.datastore.sql.cache.enabled=true, nexus.http.denyframe.enabled=true, java.net.preferIPv4Stack=true, nexus.datastore.enabled=true, path.separator=:, os.version=5.14.0-570.60.1.el9_6.x86_64, java.runtime.name=OpenJDK Runtime Environment, nexus-args=/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty.xml,/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml,/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-requestlog.xml, nexus.quartz.jobstore.jdbc=true, java.vm.name=OpenJDK 64-Bit Server VM, nexus.datastore.blobstore.metrics.enabled=true, java.vendor.url.bug=https://github.com/adoptium/adoptium-support/issues, org.sonatype.nexus.repository.httpbridge.internal.HttpBridgeModule.legacy=true, user.dir=/opt/nexus/nexus-3.86.2-01, os.arch=amd64, nexus.datastore.table.search.enabled=true, java.vm.info=mixed mode, sharing, java.vm.version=17.0.13+11, application-port-ssl=8443, java.class.version=61.0}
2025-12-10 15:54:55,121-0800 INFO  [main] *SYSTEM com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication - Starting SonatypeNexusRepositoryApplication v3.86.2-01 using Java 17.0.13 with PID 1853318 (/opt/nexus/nexus-3.86.2-01/bin/sonatype-nexus-repository-3.86.2-01.jar started by cmdeploy in /opt/nexus/nexus-3.86.2-01)
2025-12-10 15:54:55,122-0800 INFO  [main] *SYSTEM com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication - No active profile set, falling back to 1 default profile: "default"
2025-12-10 15:54:56,776-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.ApplicationLauncher - Starting nexus with edition PRO
2025-12-10 15:54:57,015-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.SpringComponentScan - Scanning for components in packages: [org.sonatype.nexus, com.sonatype.nexus]
2025-12-10 15:55:07,316-0800 INFO  [main] *SYSTEM org.sonatype.nexus.quartz.internal.QuartzSchedulerProvider - Thread-pool size: 20, Thread-pool priority: 5
2025-12-10 15:55:07,832-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.log.overrides.datastore.DatastoreLoggerOverrides - File: /opt/nexus/sonatype-work/nexus3/etc/logback/logback-overrides.xml
2025-12-10 15:55:07,835-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.log.overrides.file.LogbackLoggerOverrides - File: /opt/nexus/sonatype-work/nexus3/etc/logback/logback-overrides.xml
2025-12-10 15:55:07,868-0800 INFO  [main] *SYSTEM org.apache.shiro.nexus.NexusWebSessionManager - Global session timeout: 1800000 ms
2025-12-10 15:55:07,869-0800 INFO  [main] *SYSTEM org.apache.shiro.nexus.NexusWebSessionManager - Session-cookie prototype: name=NXSESSIONID, secure=true
2025-12-10 15:55:08,814-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle - UI plugin descriptors:
2025-12-10 15:55:08,815-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rapture
2025-12-10 15:55:08,815-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-coreui-plugin
2025-12-10 15:55:08,815-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle - ExtJS UI plugin descriptors:
2025-12-10 15:55:08,815-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rapture
2025-12-10 15:55:08,815-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-rutauth-plugin
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-proximanova-plugin
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-coreui-plugin
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-proui-plugin
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-cargo
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-composer
2025-12-10 15:55:08,816-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-onboarding-plugin
2025-12-10 15:55:08,817-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-maven
2025-12-10 15:55:08,817-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-docker
2025-12-10 15:55:08,817-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-rubygems
2025-12-10 15:55:08,817-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-npm
2025-12-10 15:55:08,817-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-nuget
2025-12-10 15:55:08,818-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-repository-pypi
2025-12-10 15:55:08,818-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-saml-plugin
2025-12-10 15:55:08,818-0800 INFO  [main] *SYSTEM org.sonatype.nexus.rapture.internal.RaptureWebResourceBundle -   nexus-analytics-plugin
2025-12-10 15:55:08,837-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.webresources.WebResourceServlet - Max-age: 30 days (2592000 seconds)
2025-12-10 15:55:08,847-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.wonderland.DownloadServiceImpl - Downloads directory: /opt/nexus/sonatype-work/nexus3/downloads
2025-12-10 15:55:09,035-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.atlas.SupportZipGeneratorImpl - Maximum included file size: 30 megabytes
2025-12-10 15:55:09,035-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.atlas.SupportZipGeneratorImpl - Maximum ZIP file size: 50 megabytes
2025-12-10 15:55:09,478-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Detected 1 engine-factories
2025-12-10 15:55:09,480-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Engine-factory: Groovy Scripting Engine v2.0; language=Groovy, version=3.0.19, names=[groovy, Groovy], mime-types=[application/x-groovy], extensions=[groovy]
2025-12-10 15:55:09,481-0800 INFO  [main] *SYSTEM org.sonatype.nexus.internal.script.ScriptEngineManagerProvider - Default language: groovy
2025-12-10 15:55:09,809-0800 INFO  [main] *SYSTEM org.hibernate.validator.internal.util.Version - HV000001: Hibernate Validator 6.2.0.Final
2025-12-10 15:55:11,098-0800 INFO  [main] *SYSTEM org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor - Inconsistent constructor declaration on bean with name 'maliciousRiskOnDiskAnalytics': single autowire-marked constructor flagged as optional - this constructor is effectively required since there is no default constructor to fall back to: public com.sonatype.analytics.internal.MaliciousRiskOnDiskAnalytics(com.sonatype.nexus.risk.visualizer.MaliciousRiskService,java.lang.Boolean)
2025-12-10 15:55:11,312-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Starting jetty
2025-12-10 15:55:11,324-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Applying configuration: file:/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty.xml
2025-12-10 15:55:11,664-0800 INFO  [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Applying configuration: file:/opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml
2025-12-10 15:55:11,678-0800 WARN  [main] *SYSTEM org.eclipse.jetty.xml.XmlConfiguration - Config error java.lang.reflect.InvocationTargetException at <Set name="KeyStorePath">
      <Call name="resolvePath" class="org.eclipse.jetty.xml.XmlConfiguration"><Arg><Property name="ssl.etc"/></Arg><Arg><Property name="jetty.sslContext.keyStorePath" default="nexus01.jks"/></Arg></Call>
    </Set> in file:///opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml
2025-12-10 15:55:11,679-0800 WARN  [main] *SYSTEM org.eclipse.jetty.xml.XmlConfiguration - Config error java.lang.reflect.InvocationTargetException at <New id="sslContextFactory" class="org.eclipse.jetty.util.ssl.SslContextFactory$Server"><Set name="Provider" property="jetty.sslContext.provider"/><Set name="KeyStorePath">
      <Call name="resolvePath" class="org.eclipse.jetty.xml.XmlConfiguration"><Arg><Property name="ssl.etc"/></Arg><Arg><Property name="jetty.sslContext.keyStorePath" default="nexus01.jks"/></Arg></Call>
    </Set><Set name="KeyStorePassword">OBF:1unr1sov1uvk1u9h1ua11uum1sov1uo7</Set><Set name="KeyStoreType" property="jetty.sslContext.keyStoreType"/><Set name="KeyStoreProvider" property="jetty.sslContext.keyStoreProvider"/><Set name="KeyManagerPassword">OBF:1unr1sov1uvk1u9h1ua11uum1sov1uo7</Set><Set name="TrustStorePath">
      <Call name="resolvePath" class="org.eclipse.jetty.xml.XmlConfiguration"><Arg><Property name="ssl.etc"/></Arg><Arg><Property name="jetty.sslContext.keyStorePath" default="nexus01.jks"/></Arg></Call>
    </Set><Set name="TrustStorePassword" property="jetty.sslContext.trustStorePassword">OBF:1unr1sov1uvk1u9h1ua11uum1sov1uo7</Set><Set name="TrustStoreType" property="jetty.sslContext.trustStoreType"/><Set name="TrustStoreProvider" property="jetty.sslContext.trustStoreProvider"/><Set name="EndpointIdentificationAlgorithm" property="jetty.sslContext.endpointIdentificationAlgorithm"/><Set name="NeedClientAuth" property="jetty.sslContext.needClientAuth"/><Set name="WantClientAuth" property="jetty.sslContext.wantClientAuth"/><Set name="useCipherSuitesOrder" property="jetty.sslContext.useCipherSuitesOrder"/><Set name="sslSessionCacheSize" property="jetty.sslContext.sslSessionCacheSize"/><Set name="sslSessionTimeout" property="jetty.sslContext.sslSessionTimeout"/><Set name="RenegotiationAllowed" property="jetty.sslContext.renegotiationAllowed"/><Set name="RenegotiationLimit" property="jetty.sslContext.renegotiationLimit"/><Set name="SniRequired" property="jetty.sslContext.sniRequired"/><Set name="IncludeProtocols">
      <Array type="java.lang.String"><Item>TLSv1.2</Item></Array>
    </Set></New> in file:///opt/nexus/nexus-3.86.2-01/etc/jetty/jetty-https.xml
2025-12-10 15:55:11,680-0800 ERROR [main] *SYSTEM org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer - Start failed
java.lang.reflect.InvocationTargetException: null
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:569)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.invokeMethod(XmlConfiguration.java:802)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.set(XmlConfiguration.java:640)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:527)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.newObj(XmlConfiguration.java:1053)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:539)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:486)
        at org.eclipse.jetty.xml.XmlConfiguration.configure(XmlConfiguration.java:388)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer.doStart(JettyServer.java:178)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer.start(JettyServer.java:133)
        at org.sonatype.nexus.bootstrap.jetty.ManagedJetty.start(ManagedJetty.java:50)
        at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:405)
        at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:394)
        at org.springframework.context.support.DefaultLifecycleProcessor$LifecycleGroup.start(DefaultLifecycleProcessor.java:586)
        at java.base/java.lang.Iterable.forEach(Iterable.java:75)
        at org.springframework.context.support.DefaultLifecycleProcessor.startBeans(DefaultLifecycleProcessor.java:364)
        at org.springframework.context.support.DefaultLifecycleProcessor.onRefresh(DefaultLifecycleProcessor.java:310)
        at org.springframework.context.support.AbstractApplicationContext.finishRefresh(AbstractApplicationContext.java:1006)
        at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:630)
        at org.sonatype.nexus.bootstrap.entrypoint.SpringComponentScan.finishBootstrapComponentScanning(SpringComponentScan.java:90)
        at org.sonatype.nexus.bootstrap.entrypoint.ApplicationLauncher.onContextRefreshed(ApplicationLauncher.java:92)
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
Caused by: java.lang.IllegalArgumentException: KeyStore Path not accessible: /opt/nexus/sonatype-work/nexus3/etc/ssl/nexus01.jks
        at org.eclipse.jetty.util.ssl.SslContextFactory.setKeyStorePath(SslContextFactory.java:655)
        ... 50 common frames omitted
2025-12-10 15:55:11,688-0800 WARN  [main] *SYSTEM org.springframework.context.annotation.AnnotationConfigApplicationContext - Exception encountered during context initialization - cancelling refresh attempt: org.springframework.context.ApplicationContextException: Failed to start bean 'org.sonatype.nexus.bootstrap.jetty.ManagedJetty'
2025-12-10 15:55:11,702-0800 WARN  [main] *SYSTEM org.springframework.beans.factory.support.DisposableBeanAdapter - Custom destroy method 'shutdown' on bean with name 'org.sonatype.nexus.thread.DatabaseStatusDelayedExecutor' propagated an exception: java.lang.NoClassDefFoundError: org/aspectj/runtime/reflect/JoinPointImpl
2025-12-10 15:55:11,762-0800 WARN  [main] *SYSTEM org.springframework.context.annotation.AnnotationConfigApplicationContext - Exception encountered during context initialization - cancelling refresh attempt: java.lang.RuntimeException: Failed to configure application
2025-12-10 15:55:11,763-0800 ERROR [main] *SYSTEM org.springframework.boot.SpringApplication - Application run failed
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
Caused by: java.lang.RuntimeException: java.lang.reflect.InvocationTargetException
        at org.sonatype.nexus.bootstrap.jetty.ManagedJetty.start(ManagedJetty.java:56)
        at org.springframework.context.support.DefaultLifecycleProcessor.doStart(DefaultLifecycleProcessor.java:405)
        ... 35 common frames omitted
Caused by: java.lang.reflect.InvocationTargetException: null
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:569)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.invokeMethod(XmlConfiguration.java:802)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.set(XmlConfiguration.java:640)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:527)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.newObj(XmlConfiguration.java:1053)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:539)
        at org.eclipse.jetty.xml.XmlConfiguration$JettyXmlConfiguration.configure(XmlConfiguration.java:486)
        at org.eclipse.jetty.xml.XmlConfiguration.configure(XmlConfiguration.java:388)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer.doStart(JettyServer.java:178)
        at org.sonatype.nexus.bootstrap.entrypoint.jetty.JettyServer.start(JettyServer.java:133)
        at org.sonatype.nexus.bootstrap.jetty.ManagedJetty.start(ManagedJetty.java:50)
        ... 36 common frames omitted
Caused by: java.lang.IllegalArgumentException: KeyStore Path not accessible: /opt/nexus/sonatype-work/nexus3/etc/ssl/nexus01.jks
        at org.eclipse.jetty.util.ssl.SslContextFactory.setKeyStorePath(SslContextFactory.java:655)
        ... 50 common frames omitted
Exception in thread "main" java.lang.reflect.InvocationTargetException
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.base/java.lang.reflect.Method.invoke(Method.java:569)
        at org.springframework.boot.loader.launch.Launcher.launch(Launcher.java:102)
        at org.springframework.boot.loader.launch.Launcher.launch(Launcher.java:64)
        at org.springframework.boot.loader.launch.JarLauncher.main(JarLauncher.java:40)
Caused by: java.lang.NoClassDefFoundError: org/springframework/boot/SpringBootExceptionHandler
        at org.springframework.boot.SpringApplication.getSpringBootExceptionHandler(SpringApplication.java:920)
        at org.springframework.boot.SpringApplication.registerLoggedException(SpringApplication.java:871)
        at org.springframework.boot.SpringApplication.reportFailure(SpringApplication.java:861)
        at org.springframework.boot.SpringApplication.handleRunFailure(SpringApplication.java:814)
        at org.springframework.boot.SpringApplication.run(SpringApplication.java:345)
        at org.springframework.boot.builder.SpringApplicationBuilder.run(SpringApplicationBuilder.java:149)
        at com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication.main(SonatypeNexusRepositoryApplication.java:48)
        ... 7 more
Caused by: java.lang.ClassNotFoundException: org.springframework.boot.SpringBootExceptionHandler
        at java.base/java.net.URLClassLoader.findClass(URLClassLoader.java:445)
        at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:592)
        at org.springframework.boot.loader.net.protocol.jar.JarUrlClassLoader.loadClass(JarUrlClassLoader.java:107)
        at org.springframework.boot.loader.launch.LaunchedClassLoader.loadClass(LaunchedClassLoader.java:91)
        at java.base/java.lang.ClassLoader.loadClass(ClassLoader.java:525)
