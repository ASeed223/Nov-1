name: 'EDR2_Demographic_Services_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

trigger: none
pr: none

schedules:
  - cron: "20 7 * * 0"
    always: true
    branches:
      include:
        - "master"
    displayName: "Weekly Sunday Midnight Scan (12:20 AM)"

resources:
  repositories:
    - repository: EDR-Demographics-Services
      type: git
      name: EDR-Demographics-Services
      ref: develop/26.1.0

pool:
  name: 'Java-Maven'

steps:
  - checkout: EDR-Demographics-Services
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
    inputs:
      nexusIqService: 'Nexus IQ Server'
      applicationId: 'EDR2_Demographics_Services_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
