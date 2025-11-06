name: 'EDR2_JBoss_Enhancements_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

trigger: none
pr: none

schedules:
  - cron: "30 7 * * 0"
    always: true
    branches:
      include:
        - "master"
    displayName: "Weekly Sunday Midnight Scan (12:30 AM)"

resources:
  repositories:
    - repository: EDR-Accounting-Services
      type: git
      name: EDR-Accounting-Services
      ref: develop/26.1.0
    - repository: EDR-Accounting-UI
      type: git
      name: EDR-Accounting-UI
      ref: develop/26.1.0
    - repository: EDR-Activities-Services
      type: git
      name: EDR-Activities-Services
      ref: develop/26.1.0
    - repository: EDR-Activities-UI
      type: git
      name: EDR-Activities-UI
      ref: develop/26.1.0
    - repository: EDR-Architecture-UI
      type: git
      name: EDR-Architecture-UI
      ref: master
    - repository: EDR-Case-Management-Services
      type: git
      name: EDR-Case-Management-Services
      ref: develop/26.1.0
    - repository: EDR-Cases-Services
      type: git
      name: EDR-Cases-Services
      ref: develop/26.1.0
    - repository: EDR-Cases-UI
      type: git
      name: EDR-Cases-UI
      ref: develop/26.1.0
    - repository: EDR-Collections-Service
      type: git
      name: EDR-Collections-Service
      ref: develop/26.1.0
    - repository: EDR-Collections-UI
      type: git
      name: EDR-Collections-UI
      ref: develop/26.1.0
    - repository: EDR-Comments-Services
      type: git
      name: EDR-Comments-Services
      ref: develop/26.1.0
    - repository: EDR-Comments-UI
      type: git
      name: EDR-Comments-UI
      ref: develop/26.1.0
    - repository: EDR-Common-Services
      type: git
      name: EDR-Common-Services
      ref: develop/26.1.0
    - repository: EDR-Compliance-Case-Integration
      type: git
      name: EDR-Compliance-Case-Integration
      ref: develop/25.4.0
    - repository: EDR-Compliance-Case-Services
      type: git
      name: EDR-Compliance-Case-Services
      ref: develop/25.4.0
    - repository: EDR-Correspondence-Services
      type: git
      name: EDR-Correspondence-Services
      ref: develop/26.1.0
    - repository: EDR-Demographics-Services
      type: git
      name: EDR-Demographics-Services
      ref: develop/26.1.0
    - repository: EDR-Demographics-UI
      type: git
      name: EDR-Demographics-UI
      ref: develop/26.1.0
    - repository: EDR-Document-Services
      type: git
      name: EDR-Document-Services
      ref: develop/26.1.0
    - repository: EDR-Document-UI
      type: git
      name: EDR-Document-UI
      ref: develop/26.1.0
    - repository: EDR-Entity-Services
      type: git
      name: EDR-Entity-Services
      ref: develop/26.1.0
    - repository: EDR-Filing-Enforcement-Services
      type: git
      name: EDR-Filing-Enforcement-Services
      ref: develop/26.1.0
    - repository: EDR-Filing-Enforcement-UI
      type: git
      name: EDR-Filing-Enforcement-UI
      ref: develop/26.1.0
    - repository: EDR-ITF-Shared-UI
      type: git
      name: EDR-ITF-Shared-UI
      ref: develop/0.3.x-branch
    - repository: EDR-POA-Builder
      type: git
      name: EDR-POA-Builder
      ref: develop/26.1.0
    - repository: EDR-POA-Services
      type: git
      name: EDR-POA-Services
      ref: develop/26.1.0
    - repository: EDR-POA-UI
      type: git
      name: EDR-POA-UI
      ref: develop/26.1.0
    - repository: EDR-Relationships-UI
      type: git
      name: EDR-Relationships-UI
      ref: develop/26.1.0

pool:
  name: 'Java-Maven'

steps:
  - checkout: EDR-Accounting-Services
    clean: true
  - checkout: EDR-Accounting-UI
    clean: true
  - checkout: EDR-Activities-Services
    clean: true
  - checkout: EDR-Activities-UI
    clean: true
  - checkout: EDR-Architecture-UI
    clean: true
  - checkout: EDR-Case-Management-Services
    clean: true
  - checkout: EDR-Cases-Services
    clean: true
  - checkout: EDR-Cases-UI
    clean: true
  - checkout: EDR-Collections-Service
    clean: true
  - checkout: EDR-Collections-UI
    clean: true
  - checkout: EDR-Comments-Services
    clean: true
  - checkout: EDR-Comments-UI
    clean: true
  - checkout: EDR-Common-Services
    clean: true
  - checkout: EDR-Compliance-Case-Integration
    clean: true
  - checkout: EDR-Compliance-Case-Services
    clean: true
  - checkout: EDR-Correspondence-Services
    clean: true
  - checkout: EDR-Demographics-Services
    clean: true
  - checkout: EDR-Demographics-UI
    clean: true
  - checkout: EDR-Document-Services
    clean: true
  - checkout: EDR-Document-UI
    clean: true
  - checkout: EDR-Entity-Services
    clean: true
  - checkout: EDR-Filing-Enforcement-Services
    clean: true
  - checkout: EDR-Filing-Enforcement-UI
    clean: true
  - checkout: EDR-ITF-Shared-UI
    clean: true
  - checkout: EDR-POA-Builder
    clean: true
  - checkout: EDR-POA-Services
    clean: true
  - checkout: EDR-POA-UI
    clean: true
  - checkout: EDR-Relationships-UI
    clean: true

  - task: JavaToolInstaller@0
    displayName: 'Use Java 17'
    inputs:
      versionSpec: 17
      jdkArchitectureOption: x64
      jdkSourceOption: PreInstalled

  - task: SonatypeIntegrations.nexus-iq-azure-extension.nexus-iq-azure-pipeline-task.NexusIqPipelineTask@2
    displayName: 'Nexus IQ Scan'
    inputs:
      nexusIqService: 'Nexus IQ Server'
      applicationId: 'EDR2_JBoss_Enhancements_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
