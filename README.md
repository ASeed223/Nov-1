name: 'EDR2_Internal_Taxpayer_Folder_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

trigger: none
pr: none

schedules:
  - cron: "25 7 * * 0"
    always: true
    branches:
      include:
        - "master"
    displayName: "Weekly Sunday Midnight Scan (12:25 AM)"

resources:
  repositories:
    - repository: EDR-AppDev-JavaApps
      type: git
      name: EDR-AppDev-JavaApps
      ref: develop/26.1
    - repository: EDR-Audit-Services
      type: git
      name: EDR-Audit-Services
      ref: develop/26.1.0
pool:
  name: 'Java-Maven'

steps:
  - checkout: EDR-AppDev-JavaApps
    path: appDev
    clean: true
  - checkout: EDR-Audit-Services
    path: auditServices
    clean: true

  # Use Java 17
  - task: JavaToolInstaller@0
    displayName: 'Use Java 17'
    inputs:
      versionSpec: 17
      jdkArchitectureOption: x64
      jdkSourceOption: PreInstalled

  # Nexus IQ Scan
  - task: SonatypeIntegrations.nexus-iq-azure-extension.nexus-iq-azure-pipeline-task.NexusIqPipelineTask@2
    displayName: 'Nexus IQ Scan'
    continueOnError: true
    inputs:
      nexusIqService: 'Nexus IQ Server'
      applicationId: 'EDR2_Internal_Taxpayer_Folder_Pipeline'
      stage: build
      scanTargets: "appDev/arch/** appDev/business_services/** appDev/ecm/** appDev/forms/** appDev/itf/** appDev/mdm/** appDev/reports/** appDev/tf/** auditServices/** !**/node_modules/** !**/how_do_i/** !**/*.js !**/*.css !**/*.json !**/*.map"
      scanPipelineWorkspace: true
