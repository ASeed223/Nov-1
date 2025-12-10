Started Sonatype Nexus PRO 3.86.2-01 (98a3285d)

-------------------------------------------------
2025-12-10 15:49:52,932-0800 INFO  [quartz-11-thread-7] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repair - Recreate component indexes for performance' [create.component.index.task] state change RUNNING -> OK
2025-12-10 15:49:52,947-0800 INFO  [quartz-11-thread-7] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Migrate trusted certificates Task
2025-12-10 15:49:52,949-0800 INFO  [quartz-11-thread-7] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Migrate trusted certificates Task' [trusted.certificates.migration] : state=RUNNING
2025-12-10 15:49:52,955-0800 INFO  [quartz-11-thread-7] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Migrate trusted certificates Task' [trusted.certificates.migration] scheduled: now
2025-12-10 15:49:52,967-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Starting migration.
2025-12-10 15:49:52,968-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - There are 42 trusted certificates to migrate.
2025-12-10 15:49:53,053-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 90:AF:2A:19:27:7A:E3:C3:6D:D6:1D:CF:96:9E:5B:1A:AE:73:94:CC was migrated successfully.
2025-12-10 15:49:53,061-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 70:E0:B6:97:E2:40:36:44:32:A2:CF:AA:0E:FD:2A:4D:C9:A5:68:80 was migrated successfully.
2025-12-10 15:49:53,063-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 49:6E:22:69:A7:44:84:10:06:8C:97:59:8D:3C:70:C1:8E:1C:FA:B1 was migrated successfully.
2025-12-10 15:49:53,065-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias C7:A5:7C:5D:01:30:D6:BC:76:F0:0B:0F:8C:83:85:18:AB:01:B2:13 was migrated successfully.
2025-12-10 15:49:53,066-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias F9:A1:86:D7:07:36:80:04:48:95:6D:1A:A7:FE:89:B6:50:29:DF:4E was migrated successfully.
2025-12-10 15:49:53,067-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 41:00:6F:AC:7F:47:B1:16:95:85:79:19:DE:A8:B5:13:19:FA:F6:C1 was migrated successfully.
2025-12-10 15:49:53,069-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 0D:E8:B0:FE:1B:30:83:98:34:0F:86:FD:1E:05:2B:AA:F5:6F:FF:08 was migrated successfully.
2025-12-10 15:49:53,071-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 7F:AB:6E:97:CA:AB:42:CE:89:3C:F2:EB:D3:6B:23:60:3D:5A:D5:E7 was migrated successfully.
2025-12-10 15:49:53,072-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias F9:A4:6F:CA:43:20:C3:B2:9A:AD:C1:FA:AE:D8:AD:1A:E7:79:09:D8 was migrated successfully.
2025-12-10 15:49:53,073-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias DF:93:2C:8E:C5:1A:82:D1:E4:3E:37:A0:67:31:0E:04:25:18:7A:0E was migrated successfully.
2025-12-10 15:49:53,075-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 58:0B:D5:65:0A:99:B0:FB:79:C7:C5:1E:61:1C:E2:D8:84:C7:0C:5E was migrated successfully.
2025-12-10 15:49:53,076-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 6B:A3:39:83:FA:97:02:A1:3D:86:6C:8C:67:59:9D:D1:93:91:E1:9B was migrated successfully.
2025-12-10 15:49:53,078-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 26:AA:D9:A6:A6:04:1E:D6:54:D9:F5:7C:B5:8D:53:B1:41:92:F9:60 was migrated successfully.
2025-12-10 15:49:53,079-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 21:6A:F1:D3:41:91:5B:7E:32:CF:49:07:ED:25:9C:A1:57:68:2F:35 was migrated successfully.
2025-12-10 15:49:53,081-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias D3:60:E7:B4:25:30:FC:8F:A5:E4:11:DA:C5:79:1E:FE:A5:3C:00:39 was migrated successfully.
2025-12-10 15:49:53,085-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 94:D4:C3:6D:55:7F:FF:F5:78:30:0B:F4:7E:C3:33:BE:B8:23:D1:32 was migrated successfully.
2025-12-10 15:49:53,087-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 05:6E:AA:F2:1E:CB:48:1C:91:DF:76:9E:2C:D5:64:23:EF:52:BC:2C was migrated successfully.
2025-12-10 15:49:53,088-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 78:20:85:79:C3:5B:A8:F0:D6:38:46:67:98:3A:1E:C3:D8:A3:1C:5C was migrated successfully.
2025-12-10 15:49:53,090-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 84:77:7D:1A:57:2B:95:FE:2C:70:C0:25:62:8E:5A:52:2F:ED:C6:B2 was migrated successfully.
2025-12-10 15:49:53,093-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 1B:65:9F:47:C6:20:8A:A0:91:C4:43:88:96:63:DB:2F:63:69:47:FF was migrated successfully.
2025-12-10 15:49:53,095-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 62:0D:75:98:E5:66:13:D0:B0:A0:EF:32:1C:60:27:9B:8F:A2:0F:90 was migrated successfully.
2025-12-10 15:49:53,097-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias F6:CB:EE:00:31:71:C5:5B:DE:C5:04:B6:1B:74:AA:C8:EC:34:24:2F was migrated successfully.
2025-12-10 15:49:53,101-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias E7:1F:20:6E:F8:04:19:33:EA:2C:E0:A8:73:FF:E0:03:41:F5:90:01 was migrated successfully.
2025-12-10 15:49:53,110-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias A1:01:BB:D0:1A:BB:31:38:B4:4E:05:A8:03:63:5B:37:68:03:02:27 was migrated successfully.
2025-12-10 15:49:53,113-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 94:BC:2A:D0:1A:CF:41:94:D4:9A:DE:44:AB:B4:42:39:8A:F6:BF:F3 was migrated successfully.
2025-12-10 15:49:53,115-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias D2:C6:48:51:76:44:0B:60:53:93:A0:DC:30:D3:4D:82:5A:99:50:B5 was migrated successfully.
2025-12-10 15:49:53,118-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias AE:AF:94:26:A5:51:6D:68:E5:32:CD:BA:E7:A6:4E:DD:5B:CF:FD:3C was migrated successfully.
2025-12-10 15:49:53,119-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias DC:0E:63:F1:6C:C5:20:94:05:FC:8E:82:FE:E1:EC:74:61:17:D7:97 was migrated successfully.
2025-12-10 15:49:53,120-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias B6:77:46:81:72:9F:57:6E:FA:C5:37:B0:02:93:10:51:31:48:D5:7B was migrated successfully.
2025-12-10 15:49:53,121-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 37:51:CB:51:3B:93:EE:67:EC:9F:18:A1:F2:AE:C1:EA:C8:7A:F9:BC was migrated successfully.
2025-12-10 15:49:53,123-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 79:55:A7:03:D1:85:81:79:AC:A2:B8:7F:B2:AF:88:66:58:27:19:5C was migrated successfully.
2025-12-10 15:49:53,125-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias B2:3A:37:FC:DB:0B:01:DE:C7:F8:4B:A4:01:6D:06:D9:50:6E:FF:58 was migrated successfully.
2025-12-10 15:49:53,126-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias AD:B3:6E:31:11:14:86:E6:E5:CC:D9:76:7C:C4:53:44:2B:B4:8E:91 was migrated successfully.
2025-12-10 15:49:53,127-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias D7:2F:47:D8:74:20:E3:F0:F9:BD:CA:C6:F0:3A:56:67:43:C4:81:B9 was migrated successfully.
2025-12-10 15:49:53,129-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 4A:66:EE:4E:4C:B0:97:18:E9:72:D2:FF:1A:0E:54:02:44:79:4B:82 was migrated successfully.
2025-12-10 15:49:53,130-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias D4:DD:14:07:5A:51:02:10:1E:5E:90:CA:E0:B9:42:4B:32:E7:0A:94 was migrated successfully.
2025-12-10 15:49:53,131-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 77:0C:F8:73:72:75:66:0C:09:E4:30:5E:52:C4:E7:48:32:8E:67:B8 was migrated successfully.
2025-12-10 15:49:53,132-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias F3:69:C1:87:1D:8C:C8:22:27:66:61:71:AE:88:2F:B9:27:32:5D:C9 was migrated successfully.
2025-12-10 15:49:53,133-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias FC:90:33:3B:DD:2F:4D:1C:0D:39:B6:73:AE:8B:B6:28:D2:29:71:ED was migrated successfully.
2025-12-10 15:49:53,135-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 61:A7:D5:EE:19:82:AB:1C:AC:EB:9F:51:13:46:B6:A2:E8:C2:01:60 was migrated successfully.
2025-12-10 15:49:53,136-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 9C:01:59:65:B4:1D:1A:2B:39:10:7E:4B:2B:01:92:20:94:98:0D:3F was migrated successfully.
2025-12-10 15:49:53,137-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - Certificate with alias 3E:E0:6A:8F:AA:9A:01:3A:08:CD:A1:0C:47:6E:8C:A0:11:31:10:94 was migrated successfully.
2025-12-10 15:49:53,140-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.ssl.plugin.tasks.TrustedCertificateMigrationService - The migration has been completed successfully, it took 173 milliseconds.
2025-12-10 15:49:53,141-0800 INFO  [quartz-11-thread-8] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Migrate trusted certificates Task' [trusted.certificates.migration] state change RUNNING -> OK
2025-12-10 15:49:53,153-0800 INFO  [quartz-11-thread-8] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Migrate Azure soft-deleted blobs to common table
2025-12-10 15:49:53,155-0800 INFO  [quartz-11-thread-8] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Migrate Azure soft-deleted blobs to common table' [azure.soft.deleted.blobstore.migration] : state=RUNNING
2025-12-10 15:49:53,160-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Migrate Azure soft-deleted blobs to common table' [azure.soft.deleted.blobstore.migration] scheduled: now
2025-12-10 15:49:53,182-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask - Task information:
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask -  ID: aa1fc19b-2a89-4719-86fe-a310950dc4a1
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask -  Type: azure.soft.deleted.blobstore.migration
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask -  Name: Migrate Azure soft-deleted blobs to common table
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask -  Description: Migrating records of soft-deleted blobs
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask - Task configuration: {.updated=2025-12-10T15:49:53.154-08:00, .name=Migrate Azure soft-deleted blobs to common table, .recoverable=true, .message=Migrating records of soft-deleted blobs, .id=aa1fc19b-2a89-4719-86fe-a310950dc4a1, .typeName=Migrate Azure soft-deleted blobs to common table, .visible=false, .typeId=azure.soft.deleted.blobstore.migration, .exposed=false, .created=2025-12-10T15:49:53.154-08:00}
2025-12-10 15:49:53,183-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/azure.soft.deleted.blobstore.migration-20251210154953181.log
2025-12-10 15:49:53,185-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.blobstore.azure.internal.upgrade.MigrateAzureSoftDeletedTask - Dropping azure_deleted_blob
2025-12-10 15:49:53,195-0800 INFO  [quartz-11-thread-9] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Migrate Azure soft-deleted blobs to common table' [azure.soft.deleted.blobstore.migration] state change RUNNING -> OK
2025-12-10 15:49:53,215-0800 INFO  [quartz-11-thread-9] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Repair - Normalize component versions for retain-n
2025-12-10 15:49:53,218-0800 INFO  [quartz-11-thread-9] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repair - Normalize component versions for retain-n' [component.normalize.version] : state=RUNNING
2025-12-10 15:49:53,226-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Repair - Normalize component versions for retain-n' [component.normalize.version] scheduled: now
2025-12-10 15:49:53,244-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.repository.content.tasks.normalize.NormalizeComponentVersionTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/component.normalize.version-20251210154953243.log
2025-12-10 15:49:53,325-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repair - Normalize component versions for retain-n' [component.normalize.version] state change RUNNING -> OK
2025-12-10 15:49:53,347-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Repository - Copy Blob Size to Asset Table
2025-12-10 15:49:53,350-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repository - Copy Blob Size to Asset Table' [repository.metrics.blob.size.copy] : state=RUNNING
2025-12-10 15:49:53,368-0800 INFO  [quartz-11-thread-10] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Repository - Copy Blob Size to Asset Table' [repository.metrics.blob.size.copy] scheduled: now
2025-12-10 15:49:53,485-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.tasks.CopyBlobSizeTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/repository.metrics.blob.size.copy-20251210154953484.log
2025-12-10 15:49:53,851-0800 INFO  [quartz-11-thread-4] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Synchronize Proprietary Names to IQ Server for repository *' [firewall.proprietary.name.sync] state change RUNNING -> WAITING (OK)
2025-12-10 15:49:54,107-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repository - Copy Blob Size to Asset Table' [repository.metrics.blob.size.copy] state change RUNNING -> OK
2025-12-10 15:49:54,259-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Retrieve external blobstore metadata
2025-12-10 15:49:54,279-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Retrieve external blobstore metadata' [external.blobstore.metadata] : state=RUNNING
2025-12-10 15:49:54,356-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Retrieve external blobstore metadata' [external.blobstore.metadata] scheduled: now
2025-12-10 15:49:54,384-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.blobstore.s3.ExternalMetadataTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/external.blobstore.metadata-20251210154954381.log
2025-12-10 15:49:54,393-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Retrieve external blobstore metadata' [external.blobstore.metadata] state change RUNNING -> OK
2025-12-10 15:49:54,419-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.scheduling.internal.upgrade.datastore.QueuingUpgradeTaskScheduler - Running failed upgrade task Remove old Reconcile Tasks
2025-12-10 15:49:54,422-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Remove old Reconcile Tasks' [old.reconcile.migration] : state=RUNNING
2025-12-10 15:49:54,430-0800 INFO  [quartz-11-thread-12] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'Remove old Reconcile Tasks' [old.reconcile.migration] scheduled: now
2025-12-10 15:49:54,450-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask - Task information:
2025-12-10 15:49:54,453-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask -  ID: 8a27cf25-e530-4d0f-a2bc-bfd651a49861
2025-12-10 15:49:54,454-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask -  Type: old.reconcile.migration
2025-12-10 15:49:54,454-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask -  Name: Remove old Reconcile Tasks
2025-12-10 15:49:54,454-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask -  Description: null
2025-12-10 15:49:54,454-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask - Task configuration: {.updated=2025-12-10T15:49:54.419-08:00, .name=Remove old Reconcile Tasks, .recoverable=true, .id=8a27cf25-e530-4d0f-a2bc-bfd651a49861, .typeName=Remove old Reconcile Tasks, .visible=false, .typeId=old.reconcile.migration, .exposed=false, .created=2025-12-10T15:49:54.419-08:00}
2025-12-10 15:49:54,454-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/old.reconcile.migration-20251210154954450.log
2025-12-10 15:49:54,472-0800 INFO  [quartz-11-thread-13] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repair - Reconcile Component Database from Blob Store - HA' [blobstore.rebuildComponentDB] removed
2025-12-10 15:49:54,474-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.reconcile.upgrade.ReconcileMigrationTask - Task 'Repair - Reconcile Component Database from Blob Store - HA' [blobstore.rebuildComponentDB] removed successfully
2025-12-10 15:49:54,475-0800 INFO  [quartz-11-thread-13] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Remove old Reconcile Tasks' [old.reconcile.migration] state change RUNNING -> OK
2025-12-10 15:49:56,609-0800 INFO  [quartz-11-thread-14] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: RedHatMaven' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,645-0800 INFO  [quartz-11-thread-15] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: nuget_org_v2' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,656-0800 INFO  [quartz-11-thread-16] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: maven-central' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,670-0800 INFO  [quartz-11-thread-17] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: m2e' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,689-0800 INFO  [quartz-11-thread-18] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: prisma_proxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,708-0800 INFO  [quartz-11-thread-19] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_GO' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,728-0800 INFO  [quartz-11-thread-20] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: confluent-io' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,742-0800 INFO  [quartz-11-thread-13] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_RedHatDockerProxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,760-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: JitPack' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,772-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: primefaces' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,792-0800 INFO  [quartz-11-thread-4] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: nuget.org-proxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,805-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: Jenkins' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,820-0800 INFO  [quartz-11-thread-9] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: pypi_proxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,835-0800 INFO  [quartz-11-thread-8] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_DockerProxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,847-0800 INFO  [quartz-11-thread-7] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: Adobe' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,871-0800 INFO  [quartz-11-thread-6] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: npm_proxy' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:56,886-0800 INFO  [quartz-11-thread-5] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_RedHatQuay' [healthcheck] state change WAITING -> RUNNING
2025-12-10 15:49:57,047-0800 INFO  [quartz-11-thread-14] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: RedHatMaven' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,052-0800 WARN  [quartz-11-thread-14] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 81fd85cf-800c-4e82-a84a-92aff5d0fbab : 'System - Repository Health Check: RedHatMaven' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,057-0800 INFO  [quartz-11-thread-14] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: RedHatMaven' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,223-0800 INFO  [quartz-11-thread-15] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: nuget_org_v2' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,227-0800 WARN  [quartz-11-thread-15] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 54ac347f-2045-43dc-95f3-0247d9afcc03 : 'System - Repository Health Check: nuget_org_v2' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,231-0800 INFO  [quartz-11-thread-15] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: nuget_org_v2' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,324-0800 INFO  [quartz-11-thread-5] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: FTB_RedHatQuay' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,326-0800 WARN  [quartz-11-thread-5] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 4b897c5e-e3b8-4240-8dc7-b4af0644e69f : 'System - Repository Health Check: FTB_RedHatQuay' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,330-0800 INFO  [quartz-11-thread-5] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_RedHatQuay' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,432-0800 INFO  [quartz-11-thread-17] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: m2e' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,436-0800 WARN  [quartz-11-thread-17] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task dadd0ae2-4964-4e4f-abc7-070ad7def363 : 'System - Repository Health Check: m2e' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,443-0800 INFO  [quartz-11-thread-17] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: m2e' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,514-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: apt
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: cargo
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: docker
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: helm
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: maven2
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: npm
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: nuget
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: r
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: raw
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: rubygems
2025-12-10 15:49:57,515-0800 INFO  [main] *SYSTEM com.sonatype.nexus.replication.internal.ReplicationChecks - Added Replication default supported format: conan
2025-12-10 15:49:57,519-0800 INFO  [main] *SYSTEM com.sonatype.nexus.bootstrap.entrypoint.pro.SonatypeNexusRepositoryApplication - Started SonatypeNexusRepositoryApplication in 34.919 seconds (process running for 35.665)
2025-12-10 15:49:57,523-0800 INFO  [quartz-11-thread-18] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: prisma_proxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,524-0800 WARN  [quartz-11-thread-18] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 26f2a288-373e-4ff0-9045-d33787321c8e : 'System - Repository Health Check: prisma_proxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,526-0800 INFO  [quartz-11-thread-18] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: prisma_proxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,597-0800 INFO  [quartz-11-thread-19] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: FTB_GO' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,599-0800 WARN  [quartz-11-thread-19] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task baef6504-dae5-4ce1-b3ad-14297c8fe25c : 'System - Repository Health Check: FTB_GO' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,611-0800 INFO  [quartz-11-thread-19] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_GO' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,689-0800 INFO  [quartz-11-thread-6] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: npm_proxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,691-0800 WARN  [quartz-11-thread-6] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task df29745c-ad6f-4a31-a2b2-f1b88e0f286d : 'System - Repository Health Check: npm_proxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,699-0800 INFO  [quartz-11-thread-6] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: npm_proxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,772-0800 INFO  [quartz-11-thread-20] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: confluent-io' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,775-0800 WARN  [quartz-11-thread-20] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task c13aa92e-4893-40bb-a94c-12b5fb736260 : 'System - Repository Health Check: confluent-io' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,780-0800 INFO  [quartz-11-thread-20] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: confluent-io' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,854-0800 INFO  [quartz-11-thread-7] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: Adobe' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,857-0800 WARN  [quartz-11-thread-7] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task ef9b1273-03ee-4db1-a826-e91e40dcabd1 : 'System - Repository Health Check: Adobe' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,864-0800 INFO  [quartz-11-thread-7] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: Adobe' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:57,942-0800 INFO  [quartz-11-thread-16] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: maven-central' [healthcheck] scheduled: hourly
2025-12-10 15:49:57,944-0800 WARN  [quartz-11-thread-16] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 8da7cff8-b25b-48eb-93dc-a6395b29813b : 'System - Repository Health Check: maven-central' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:57,946-0800 INFO  [quartz-11-thread-16] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: maven-central' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,043-0800 INFO  [quartz-11-thread-13] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: FTB_RedHatDockerProxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,046-0800 WARN  [quartz-11-thread-13] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 7f6bebec-c0cf-45d6-a663-a1bd67728e35 : 'System - Repository Health Check: FTB_RedHatDockerProxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,052-0800 INFO  [quartz-11-thread-13] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_RedHatDockerProxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,125-0800 INFO  [quartz-11-thread-4] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: nuget.org-proxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,127-0800 WARN  [quartz-11-thread-4] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task ea64f295-0cfd-4aea-9b81-3549de89f7b1 : 'System - Repository Health Check: nuget.org-proxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,129-0800 INFO  [quartz-11-thread-4] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: nuget.org-proxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,198-0800 INFO  [quartz-11-thread-8] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: FTB_DockerProxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,202-0800 WARN  [quartz-11-thread-8] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 8ce80ccd-9300-464c-b85b-4e2ad0656a88 : 'System - Repository Health Check: FTB_DockerProxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,209-0800 INFO  [quartz-11-thread-8] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: FTB_DockerProxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,281-0800 INFO  [quartz-11-thread-12] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: JitPack' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,284-0800 WARN  [quartz-11-thread-12] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task 20eddaa1-2657-40a1-8710-07c05b4e0968 : 'System - Repository Health Check: JitPack' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,291-0800 INFO  [quartz-11-thread-12] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: JitPack' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,371-0800 INFO  [quartz-11-thread-9] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: pypi_proxy' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,374-0800 WARN  [quartz-11-thread-9] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task d600f122-fbde-4c98-8321-68f7adcf2801 : 'System - Repository Health Check: pypi_proxy' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,377-0800 INFO  [quartz-11-thread-9] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: pypi_proxy' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,450-0800 INFO  [quartz-11-thread-10] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: Jenkins' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,452-0800 WARN  [quartz-11-thread-10] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task d652f384-9b8a-497f-b072-e5bc65aa900b : 'System - Repository Health Check: Jenkins' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,459-0800 INFO  [quartz-11-thread-10] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: Jenkins' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,528-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.distributed.internal.tasks.ClusteredTaskSchedulerImpl - Task 'System - Repository Health Check: primefaces' [healthcheck] scheduled: hourly
2025-12-10 15:49:58,529-0800 WARN  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskJob - Task ee9e797d-d4b8-402e-9c0b-3d958ee5ac52 : 'System - Repository Health Check: primefaces' [healthcheck] execution failure
javax.net.ssl.SSLHandshakeException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.ssl.Alert.createSSLException(Alert.java:131)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:383)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:326)
        at java.base/sun.security.ssl.TransportContext.fatal(TransportContext.java:321)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:654)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.onCertificate(CertificateMessage.java:473)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.consume(CertificateMessage.java:369)
        at java.base/sun.security.ssl.SSLHandshake.consume(SSLHandshake.java:396)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:480)
        at java.base/sun.security.ssl.HandshakeContext.dispatch(HandshakeContext.java:458)
        at java.base/sun.security.ssl.TransportContext.dispatch(TransportContext.java:206)
        at java.base/sun.security.ssl.SSLTransport.decode(SSLTransport.java:172)
        at java.base/sun.security.ssl.SSLSocketImpl.decode(SSLSocketImpl.java:1510)
        at java.base/sun.security.ssl.SSLSocketImpl.readHandshakeRecord(SSLSocketImpl.java:1425)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:455)
        at java.base/sun.security.ssl.SSLSocketImpl.startHandshake(SSLSocketImpl.java:426)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.createLayeredSocket(SSLConnectionSocketFactory.java:436)
        at org.apache.http.conn.ssl.SSLConnectionSocketFactory.connectSocket(SSLConnectionSocketFactory.java:384)
        at org.sonatype.nexus.internal.httpclient.NexusSSLConnectionSocketFactory.connectSocket(NexusSSLConnectionSocketFactory.java:89)
        at org.apache.http.impl.conn.DefaultHttpClientConnectionOperator.connect(DefaultHttpClientConnectionOperator.java:142)
        at org.apache.http.impl.conn.PoolingHttpClientConnectionManager.connect(PoolingHttpClientConnectionManager.java:376)
        at org.apache.http.impl.execchain.MainClientExec.establishRoute(MainClientExec.java:393)
        at org.apache.http.impl.execchain.MainClientExec.execute(MainClientExec.java:236)
        at org.apache.http.impl.execchain.ProtocolExec.execute(ProtocolExec.java:186)
        at org.apache.http.impl.execchain.RetryExec.execute(RetryExec.java:89)
        at org.apache.http.impl.execchain.RedirectExec.execute(RedirectExec.java:110)
        at org.apache.http.impl.client.InternalHttpClient.doExecute(InternalHttpClient.java:185)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:83)
        at org.apache.http.impl.client.CloseableHttpClient.execute(CloseableHttpClient.java:56)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.execute(HdsServiceImpl.java:276)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.doGet(HdsServiceImpl.java:224)
        at com.sonatype.nexus.plugins.healthcheck.service.impl.HdsServiceImpl.getNextRunDeltas(HdsServiceImpl.java:104)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doDeltaCheck(HealthCheckTask.java:249)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.doRunSafe(HealthCheckTask.java:145)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:109)
        at com.sonatype.nexus.plugins.healthcheck.task.HealthCheckTask.execute(HealthCheckTask.java:1)
        at org.sonatype.nexus.scheduling.TaskSupport.call(TaskSupport.java:107)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.doExecute(QuartzTaskJob.java:147)
        at org.sonatype.nexus.quartz.internal.task.QuartzTaskJob.execute(QuartzTaskJob.java:110)
        at org.quartz.core.JobRunShell.run(JobRunShell.java:202)
        at org.sonatype.nexus.quartz.internal.QuartzThreadPool.lambda$0(QuartzThreadPool.java:145)
        at org.sonatype.nexus.thread.internal.MDCAwareRunnable.run(MDCAwareRunnable.java:40)
        at org.apache.shiro.subject.support.SubjectRunnable.doRun(SubjectRunnable.java:120)
        at org.apache.shiro.subject.support.SubjectRunnable.run(SubjectRunnable.java:108)
        at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:539)
        at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:840)
Caused by: sun.security.validator.ValidatorException: PKIX path building failed: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:439)
        at java.base/sun.security.validator.PKIXValidator.engineValidate(PKIXValidator.java:306)
        at java.base/sun.security.validator.Validator.validate(Validator.java:264)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkTrusted(X509TrustManagerImpl.java:231)
        at java.base/sun.security.ssl.X509TrustManagerImpl.checkServerTrusted(X509TrustManagerImpl.java:132)
        at java.base/sun.security.ssl.CertificateMessage$T12CertificateConsumer.checkServerCerts(CertificateMessage.java:638)
        ... 44 common frames omitted
Caused by: sun.security.provider.certpath.SunCertPathBuilderException: unable to find valid certification path to requested target
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.build(SunCertPathBuilder.java:148)
        at java.base/sun.security.provider.certpath.SunCertPathBuilder.engineBuild(SunCertPathBuilder.java:129)
        at java.base/java.security.cert.CertPathBuilder.build(CertPathBuilder.java:297)
        at java.base/sun.security.validator.PKIXValidator.doBuild(PKIXValidator.java:434)
        ... 49 common frames omitted
2025-12-10 15:49:58,536-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'System - Repository Health Check: primefaces' [healthcheck] state change RUNNING -> WAITING (FAILED)
2025-12-10 15:49:58,987-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repository Metrics initialize scheduler' [repository.metrics.initialize.scheduler] state change WAITING -> RUNNING
2025-12-10 15:49:58,992-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask - Task information:
2025-12-10 15:49:58,993-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask -  ID: 0211cb14-2d3c-4336-97c6-aff531a54ab7
2025-12-10 15:49:58,993-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask -  Type: repository.metrics.initialize.scheduler
2025-12-10 15:49:58,994-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask -  Name: Repository Metrics initialize scheduler
2025-12-10 15:49:58,994-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask -  Description: Process repository metrics initialize schedules
2025-12-10 15:49:58,994-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask - Task configuration: {.updated=2025-12-10T15:49:53.979-08:00, .name=Repository Metrics initialize scheduler, .recoverable=false, .message=Process repository metrics initialize schedules, .id=0211cb14-2d3c-4336-97c6-aff531a54ab7, .typeName=Repository Metrics initialize scheduler, .visible=false, .typeId=repository.metrics.initialize.scheduler, .exposed=false, .created=2025-12-10T15:49:53.979-08:00}
2025-12-10 15:49:58,994-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.repository.content.store.metrics.RepositoryMetricsInitTask - Task log: /opt/nexus/sonatype-work/nexus3/log/tasks/repository.metrics.initialize.scheduler-20251210154958991.log
2025-12-10 15:49:59,682-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Repository Metrics initialize scheduler' [repository.metrics.initialize.scheduler] state change RUNNING -> OK
2025-12-10 15:50:21,909-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Malicious Risk On Disk - Auto enable Health Check for proxy repositories on startup' [malicious-risk-on-disk-auto-enable-rhc] state change WAITING -> RUNNING
2025-12-10 15:50:21,911-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCTask - Starting malicious-risk-on-disk-auto-enable-rhc task
2025-12-10 15:50:21,912-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCTask - Found 17 proxy repositories
2025-12-10 15:50:21,915-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'RedHatMaven' repository.
2025-12-10 15:50:21,916-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'nuget_org_v2' repository.
2025-12-10 15:50:21,917-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'maven-central' repository.
2025-12-10 15:50:21,918-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'm2e' repository.
2025-12-10 15:50:21,919-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'prisma_proxy' repository.
2025-12-10 15:50:21,919-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'FTB_GO' repository.
2025-12-10 15:50:21,920-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'confluent-io' repository.
2025-12-10 15:50:21,921-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'FTB_RedHatDockerProxy' repository.
2025-12-10 15:50:21,922-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'JitPack' repository.
2025-12-10 15:50:21,923-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'primefaces' repository.
2025-12-10 15:50:21,924-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'nuget.org-proxy' repository.
2025-12-10 15:50:21,924-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'Jenkins' repository.
2025-12-10 15:50:21,925-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'pypi_proxy' repository.
2025-12-10 15:50:21,926-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'FTB_DockerProxy' repository.
2025-12-10 15:50:21,926-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'Adobe' repository.
2025-12-10 15:50:21,927-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'npm_proxy' repository.
2025-12-10 15:50:21,928-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCService - Should not enable health check for 'FTB_RedHatQuay' repository.
2025-12-10 15:50:21,928-0800 INFO  [quartz-11-thread-11] *TASK com.sonatype.nexus.risk.riskondisk.MaliciousRiskOnDiskAutoEnableRHCTask - Completed malicious-risk-on-disk-auto-enable-rhc task
2025-12-10 15:50:21,929-0800 INFO  [quartz-11-thread-11] *TASK org.sonatype.nexus.quartz.internal.task.QuartzTaskInfo - Task 'Malicious Risk On Disk - Auto enable Health Check for proxy repositories on startup' [malicious-risk-on-disk-auto-enable-rhc] state change RUNNING -> WAITING (OK)
