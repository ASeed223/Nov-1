name: 'EDR2_Repos_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

trigger: none
pr: none

schedules:
  - cron: "20 8 * * 0"
    always: true
    branches:
      include:
        - "master"
    displayName: "Weekly Sunday Midnight Scan (01:20 AM)"

resources:
  repositories:
    - repository: EDR-Collections-Batch
      type: git
      name: EDR-Collections-Batch
      ref: develop/25.4.3.1
    - repository: EDR-Collections-Integration
      type: git
      name: EDR-Collections-Integration
      ref: develop/26.1.0
    - repository: EDR-Collections-Persistence
      type: git
      name: EDR-Collections-Persistence
      ref: develop/26.1.0
    - repository: EDR-ECM-Services
      type: git
      name: EDR-ECM-Services
      ref: develop/26.1.0
    - repository: EDR-Electronic-IA-Service
      type: git
      name: EDR-Electronic-IA-Service
      ref: develop/26.1.0
    - repository: EDR-Electronic-IA-UI
      type: git
      name: EDR-Electronic-IA-UI
      ref: develop/24.3.0
    - repository: EDR-Emulator-Services
      type: git
      name: EDR-Emulator-Services
      ref: develop/26.1.0
    - repository: EDR-Filing-Enforcement-Batch
      type: git
      name: EDR-Filing-Enforcement-Batch
      ref: develop/26.1.0
    - repository: EDR-Filing-Enforcement-Persistence
      type: git
      name: EDR-Filing-Enforcement-Persistence
      ref: develop/26.1.0
    - repository: EDR-Filing-Services
      type: git
      name: EDR-Filing-Services
      ref: develop/22.4.0
    - repository: EDR-Fraud-Scoring-Service
      type: git
      name: EDR-Fraud-Scoring-Service
      ref: develop/24.3.0
    - repository: EDR-Message-Repeater-Demographics
      type: git
      name: EDR-Message-Repeater-Demographics
      ref: develop/26.1.0
    - repository: EDR-MyFTB-Fillable-Forms
      type: git
      name: EDR-MyFTB-Fillable-Forms
      ref: develop
    - repository: EDR-Offer-In-Compromise-Service
      type: git
      name: EDR-Offer-In-Compromise-Service
      ref: develop/24.1.0
    - repository: EDR-Offer-In-Compromise-UI
      type: git
      name: EDR-Offer-In-Compromise-UI
      ref: develop/24.1.0
    - repository: EDR-PDF-Services
      type: git
      name: EDR-PDF-Services
      ref: develop/26.1.0
    - repository: EDR-Persistence-EOD
      type: git
      name: EDR-Persistence-EOD
      ref: develop/25.4.0
    - repository: EDR-ThirdParty-Services
      type: git
      name: EDR-ThirdParty-Services
      ref: develop/26.3.0
    - repository: EDR-ThirdParty-UI
      type: git
      name: EDR-ThirdParty-UI
      ref: develop/26.3.0
    - repository: EDR-TPF-UI
      type: git
      name: EDR-TPF-UI
      ref: develop/26.3.0
    - repository: EDR-Withholding-Return-Batch
      type: git
      name: EDR-Withholding-Return-Batch
      ref: develop/26.1.0
    - repository: EDR-Withholding-Return-Persistence
      type: git
      name: EDR-Withholding-Return-Persistence
      ref: develop/25.4.0
    - repository: EDR-Invariant-Legacy-Archive
      type: git
      name: EDR-Invariant-Legacy-Archive
      ref: develop/26.1.0
    - repository: EDR-Invariant-Legacy-Conversion
      type: git
      name: EDR-Invariant-Legacy-Conversion
      ref: develop/26.1.0
    - repository: IVR Mindful CallBack
      type: git
      name: IVR Mindful CallBack
      ref: develop/26.1.0
    - repository: EDR-Knowledge-Library
      type: git
      name: EDR-Knowledge-Library
      ref: develop/26.1.0
    - repository: EDR-Online-Help
      type: git
      name: EDR-Online-Help
      ref: develop/26.1.0
    - repository: EDR-Open-Case-Doc
      type: git
      name: EDR-Open-Case-Doc
      ref: develop/26.1.0
    - repository: EDR-Batch-Client
      type: git
      name: EDR-Batch-Client
      ref: develop/26.1.0
    - repository: EDR-Case-Archive
      type: git
      name: EDR-Case-Archive
      ref: develop/26.1.0
    - repository: EDR-Case-Document-API
      type: git
      name: EDR-Case-Document-API
      ref: develop/26.1.0

pool:
  name: 'Java-Maven'

steps:
  # Check out all repositories
  - checkout: EDR-Collections-Batch
    clean: true
  - checkout: EDR-Collections-Integration
    clean: true
  - checkout: EDR-Collections-Persistence
    clean: true
  - checkout: EDR-ECM-Services
    clean: true
  - checkout: EDR-Electronic-IA-Service
    clean: true
  - checkout: EDR-Electronic-IA-UI
    clean: true
  - checkout: EDR-Emulator-Services
    clean: true
  - checkout: EDR-Filing-Enforcement-Batch
    clean: true
  - checkout: EDR-Filing-Enforcement-Persistence
    clean: true
  - checkout: EDR-Filing-Services
    clean: true
  - checkout: EDR-Fraud-Scoring-Service
    clean: true
  - checkout: EDR-Message-Repeater-Demographics
    clean: true
  - checkout: EDR-MyFTB-Fillable-Forms
    clean: true
  - checkout: EDR-Offer-In-Compromise-Service
    clean: true
  - checkout: EDR-Offer-In-Compromise-UI
    clean: true
  - checkout: EDR-PDF-Services
    clean: true
  - checkout: EDR-Persistence-EOD
    clean: true
  - checkout: EDR-ThirdParty-Services
    clean: true
  - checkout: EDR-ThirdParty-UI
    clean: true
  - checkout: EDR-TPF-UI
    clean: true
  - checkout: EDR-Withholding-Return-Batch
    clean: true
  - checkout: EDR-Withholding-Return-Persistence
    clean: true
  - checkout: EDR-Invariant-Legacy-Archive
    clean: true
  - checkout: EDR-Invariant-Legacy-Conversion
    clean: true
  - checkout: IVR Mindful CallBack
    clean: true
  - checkout: EDR-Knowledge-Library
    clean: true
  - checkout: EDR-Online-Help
    clean: true
  - checkout: EDR-Open-Case-Doc
    clean: true
  - checkout: EDR-Batch-Client
    clean: true
  - checkout: EDR-Case-Archive
    clean: true
  - checkout: EDR-Case-Document-API
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
      applicationId: 'EDR2_Repos_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
