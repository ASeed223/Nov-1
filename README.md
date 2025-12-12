2025-12-12 10:48:19,857-0800 ERROR [FelixStartLevel] *SYSTEM org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl - Missing migrations: [ConanV2UpgradeStep_2_8, MalwareRemediatorTaskMigrationStep_2_9, MalwareRemediatorMigrationStep_2_10, BlobstoreSecretsMigrationStep_2_11, HuggingFaceProxyDatabaseMigrationStep_2_12, CoordinateMigrationStep_2_13, RemoveDistributedCooperationMigrationStep_2_14, RemoveLog4JVisualizer_2_15, SearchCapabilityStep_2_16, TrustedCertificatesMigrationStep_2_17, NodeHeartBeatMigrationStep_2_17_1, ConanCleanupMigrationStep_2_18]
2025-12-12 10:48:19,857-0800 ERROR [FelixStartLevel] *SYSTEM org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl - Missing migrations: [ConanV2UpgradeStep_2_8, MalwareRemediatorTaskMigrationStep_2_9, MalwareRemediatorMigrationStep_2_10, BlobstoreSecretsMigrationStep_2_11, HuggingFaceProxyDatabaseMigrationStep_2_12, CoordinateMigrationStep_2_13, RemoveDistributedCooperationMigrationStep_2_14, RemoveLog4JVisualizer_2_15, SearchCapabilityStep_2_16, TrustedCertificatesMigrationStep_2_17, NodeHeartBeatMigrationStep_2_17_1, ConanCleanupMigrationStep_2_18]
2025-12-12 10:48:19,859-0800 ERROR [FelixStartLevel] *SYSTEM org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl - Failed transition: NEW -> STARTED
org.sonatype.nexus.upgrade.datastore.UpgradeException: The database appears to be from a later version of Nexus Repository
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.checkSchemaVersionIsAcceptable(UpgradeManagerImpl.java:204)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.migrate(UpgradeManagerImpl.java:89)
        at org.sonatype.nexus.upgrade.datastore.UpgradeManager.migrate(UpgradeManager.java:34)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:62)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.MethodInvocationAction.run(MethodInvocationAction.java:39)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:206)
        at org.sonatype.nexus.common.stateguard.TransitionsInterceptor.invoke(TransitionsInterceptor.java:57)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:210)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:121)
        at org.sonatype.nexus.extender.NexusContextListener.moveToPhase(NexusContextListener.java:334)
        at org.sonatype.nexus.extender.NexusContextListener.frameworkEvent(NexusContextListener.java:231)
        at org.apache.felix.framework.Felix.setActiveStartLevel(Felix.java:1597)
        at org.apache.felix.framework.FrameworkStartLevelImpl.run(FrameworkStartLevelImpl.java:308)
        at java.base/java.lang.Thread.run(Thread.java:840)
2025-12-12 10:48:19,861-0800 ERROR [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusContextListener - Failed to start nexus
org.sonatype.nexus.upgrade.datastore.UpgradeException: The database appears to be from a later version of Nexus Repository
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.checkSchemaVersionIsAcceptable(UpgradeManagerImpl.java:204)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.migrate(UpgradeManagerImpl.java:89)
        at org.sonatype.nexus.upgrade.datastore.UpgradeManager.migrate(UpgradeManager.java:34)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:62)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.MethodInvocationAction.run(MethodInvocationAction.java:39)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:206)
        at org.sonatype.nexus.common.stateguard.TransitionsInterceptor.invoke(TransitionsInterceptor.java:57)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:210)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:121)
        at org.sonatype.nexus.extender.NexusContextListener.moveToPhase(NexusContextListener.java:334)
        at org.sonatype.nexus.extender.NexusContextListener.frameworkEvent(NexusContextListener.java:231)
        at org.apache.felix.framework.Felix.setActiveStartLevel(Felix.java:1597)
        at org.apache.felix.framework.FrameworkStartLevelImpl.run(FrameworkStartLevelImpl.java:308)
        at java.base/java.lang.Thread.run(Thread.java:840)
2025-12-12 10:48:19,863-0800 ERROR [FelixStartLevel] *SYSTEM Felix - Framework listener delivery error.
java.lang.RuntimeException: org.sonatype.nexus.upgrade.datastore.UpgradeException: The database appears to be from a later version of Nexus Repository
        at org.sonatype.nexus.extender.NexusContextListener.frameworkEvent(NexusContextListener.java:243)
        at org.apache.felix.framework.Felix.setActiveStartLevel(Felix.java:1597)
        at org.apache.felix.framework.FrameworkStartLevelImpl.run(FrameworkStartLevelImpl.java:308)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: org.sonatype.nexus.upgrade.datastore.UpgradeException: The database appears to be from a later version of Nexus Repository
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.checkSchemaVersionIsAcceptable(UpgradeManagerImpl.java:204)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeManagerImpl.migrate(UpgradeManagerImpl.java:89)
        at org.sonatype.nexus.upgrade.datastore.UpgradeManager.migrate(UpgradeManager.java:34)
        at org.sonatype.nexus.upgrade.datastore.internal.UpgradeServiceImpl.doStart(UpgradeServiceImpl.java:62)
        at org.sonatype.nexus.common.stateguard.StateGuardLifecycleSupport.start(StateGuardLifecycleSupport.java:69)
        at org.sonatype.nexus.common.stateguard.MethodInvocationAction.run(MethodInvocationAction.java:39)
        at org.sonatype.nexus.common.stateguard.StateGuard$TransitionImpl.run(StateGuard.java:206)
        at org.sonatype.nexus.common.stateguard.TransitionsInterceptor.invoke(TransitionsInterceptor.java:57)
        at org.sonatype.nexus.extender.NexusLifecycleManager.startComponent(NexusLifecycleManager.java:210)
        at org.sonatype.nexus.extender.NexusLifecycleManager.to(NexusLifecycleManager.java:121)
        at org.sonatype.nexus.extender.NexusContextListener.moveToPhase(NexusContextListener.java:334)
        at org.sonatype.nexus.extender.NexusContextListener.frameworkEvent(NexusContextListener.java:231)
        ... 3 common frames omitted
2025-12-12 10:48:19,873-0800 INFO  [FelixStartLevel] *SYSTEM com.sonatype.nexus.common.ProCommonActivator - Stopping pro-common bundle...
2025-12-12 10:48:19,883-0800 INFO  [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusContextListener - Uptime: 30 seconds and 951 milliseconds (nexus-pro-edition/3.75.0.06)
2025-12-12 10:48:19,884-0800 INFO  [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Shutting down
2025-12-12 10:48:19,886-0800 INFO  [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop RESTORE
2025-12-12 10:48:19,886-0800 INFO  [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop STORAGE
2025-12-12 10:48:19,907-0800 INFO  [FelixStartLevel] *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Shutdown initiated...
2025-12-12 10:48:19,943-0800 INFO  [FelixStartLevel] *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Shutdown completed.
2025-12-12 10:48:19,943-0800 INFO  [FelixStartLevel] *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop KERNEL
[cmdeploy@lxpd208 nexus]$ tail -f /opt/nexus/sonatype-work/nexus3/log/nexus.log
        at org.sonatype.nexus.extender.NexusContextListener.frameworkEvent(NexusContextListener.java:231)
        ... 3 common frames omitted
2025-12-12 10:48:19,873-0800 INFO  [FelixStartLevel]  *SYSTEM com.sonatype.nexus.common.ProCommonActivator - Stopping pro-common bundle...
2025-12-12 10:48:19,883-0800 INFO  [FelixStartLevel]  *SYSTEM org.sonatype.nexus.extender.NexusContextListener - Uptime: 30 seconds and 951 milliseconds (nexus-pro-edition/3.75.0.06)
2025-12-12 10:48:19,884-0800 INFO  [FelixStartLevel]  *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Shutting down
2025-12-12 10:48:19,886-0800 INFO  [FelixStartLevel]  *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop RESTORE
2025-12-12 10:48:19,886-0800 INFO  [FelixStartLevel]  *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop STORAGE
2025-12-12 10:48:19,907-0800 INFO  [FelixStartLevel]  *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Shutdown initiated...
2025-12-12 10:48:19,943-0800 INFO  [FelixStartLevel]  *SYSTEM com.zaxxer.hikari.HikariDataSource - nexus - Shutdown completed.
2025-12-12 10:48:19,943-0800 INFO  [FelixStartLevel]  *SYSTEM org.sonatype.nexus.extender.NexusLifecycleManager - Stop KERNEL
