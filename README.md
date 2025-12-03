name: 'EDR2_IVR_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

trigger: none
pr: none

schedules:
  - cron: "25 8 * * 0"
    always: true
    branches:
      include:
        - "master"
    displayName: "Weekly Sunday Midnight Scan (01:25 AM)"

resources:
  repositories:
    - repository: IVR Rewrite Project
      type: git
      name: IVR Rewrite Project
      ref: master
    - repository: IVR_Rewrite_Resources
      type: git
      name: IVR_Rewrite_Resources
      ref: master

pool:
  name: 'Java-Maven'

steps:
  # Check out both repositories
  - checkout: IVR Rewrite Project
    clean: true
  - checkout: IVR_Rewrite_Resources
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
      applicationId: 'EDR2_IVR_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
