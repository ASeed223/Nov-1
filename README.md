name: 'EDR1_Repos_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

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
    - repository: EDR-Infrastructure-PRPC
      type: git
      name: EDR-Infrastructure-PRPC
      ref: master
    - repository: EDR-Invariant-DataTools
      type: git
      name: EDR-Invariant-DataTools
      ref: master

pool:
  name: 'Java-Maven'

steps:
  # Check out both repositories
  - checkout: EDR-Infrastructure-PRPC
    clean: true
  - checkout: EDR-Invariant-DataTools
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
      applicationId: 'EDR1_Repos_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
