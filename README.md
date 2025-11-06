name: 'EDR1_Repos_Nexus_IQ-Scan_Report $(date:yyyyMMdd)$(rev:.r)'

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
    - repository: Arisant
      type: git
      name: Arisant
      ref: master
    - repository: EDL-Utilities
      type: git
      name: EDL-Utilities
      ref: master
    - repository: EDR-AEM-Utilities
      type: git
      name: EDR-AEM-Utilities
      ref: master
    - repository: EDR-AMZ-Utilities
      type: git
      name: EDR-AMZ-Utilities
      ref: master
    - repository: EDR-AnalyticModels-Audit
      type: git
      name: EDR-AnalyticModels-Audit
      ref: master
    - repository: EDR-AnalyticModels-Collections
      type: git
      name: EDR-AnalyticModels-Collections
      ref: master
    - repository: EDR-AnalyticModels-FE
      type: git
      name: EDR-AnalyticModels-FE
      ref: master
    - repository: EDR-AnalyticModels-Legal
      type: git
      name: EDR-AnalyticModels-Legal
      ref: master
    - repository: EDR-AnalyticModels-Pipelines
      type: git
      name: EDR-AnalyticModels-Pipelines
      ref: master
    - repository: EDR-AnalyticModels-RA
      type: git
      name: EDR-AnalyticModels-RA
      ref: master
    - repository: EDR-AppDev-Forms
      type: git
      name: EDR-AppDev-Forms
      ref: master
    - repository: EDR-AppDev-Middleware
      type: git
      name: EDR-AppDev-Middleware
      ref: master
    - repository: EDR-AppDev-NonJava
      type: git
      name: EDR-AppDev-NonJava
      ref: master
    - repository: EDR-Architecture-Sample
      type: git
      name: EDR-Architecture-Sample
      ref: master
    - repository: EDR-Automation-Test
      type: git
      name: EDR-Automation-Test
      ref: master
    - repository: EDR-Batch-Client
      type: git
      name: EDR-Batch-Client
      ref: master
    - repository: EDR-Case-Archive
      type: git
      name: EDR-Case-Archive
      ref: master
    - repository: EDR-Case-Document-API
      type: git
      name: EDR-Case-Document-API
      ref: master
    - repository: EDR-Case-Document-Templates
      type: git
      name: EDR-Case-Document-Templates
      ref: master
    - repository: EDR-CnfgMgmt-Ansible
      type: git
      name: EDR-CnfgMgmt-Ansible
      ref: master
    - repository: EDR-CnfgMgmt-Pipelines
      type: git
      name: EDR-CnfgMgmt-Pipelines
      ref: master
    - repository: EDR-Collections-Batch
      type: git
      name: EDR-Collections-Batch
      ref: master
    - repository: EDR-Collections-Integration
      type: git
      name: EDR-Collections-Integration
      ref: master
    - repository: EDR-Collections-Persistence
      type: git
      name: EDR-Collections-Persistence
      ref: master
    - repository: EDR-Data-ETL
      type: git
      name: EDR-Data-ETL
      ref: master
    - repository: EDR-Data-MDM
      type: git
      name: EDR-Data-MDM
      ref: master
    - repository: EDR-Data-PySpark
      type: git
      name: EDR-Data-PySpark
      ref: master
    - repository: EDR-Data-Virtualization
      type: git
      name: EDR-Data-Virtualization
      ref: master
    - repository: EDR-Data-Visualization
      type: git
      name: EDR-Data-Visualization
      ref: master
    - repository: EDR-EASE-Okta-MyFTB-Integration
      type: git
      name: EDR-EASE-Okta-MyFTB-Integration
      ref: master
    - repository: EDR-ECM-Services
      type: git
      name: EDR-ECM-Services
      ref: master
    - repository: EDR-Electronic-IA-Service
      type: git
      name: EDR-Electronic-IA-Service
      ref: master
    - repository: EDR-Electronic-IA-UI
      type: git
      name: EDR-Electronic-IA-UI
      ref: master
    - repository: EDR-Emulator-Services
      type: git
      name: EDR-Emulator-Services
      ref: master
    - repository: EDR-Filing-Enforcement-Batch
      type: git
      name: EDR-Filing-Enforcement-Batch
      ref: master
    - repository: EDR-Filing-Enforcement-Persistence
      type: git
      name: EDR-Filing-Enforcement-Persistence
      ref: master
    - repository: EDR-Filing-Services
      type: git
      name: EDR-Filing-Services
      ref: master
    - repository: EDR-Fraud-Scoring-Service
      type: git
      name: EDR-Fraud-Scoring-Service
      ref: master
    - repository: EDR-Health-Checks-Dashboard
      type: git
      name: EDR-Health-Checks-Dashboard
      ref: master
    - repository: EDR-Hearing-Services
      type: git
      name: EDR-Hearing-Services
      ref: master
    - repository: EDR-iCapture
      type: git
      name: EDR-iCapture
      ref: master
    - repository: EDR-Infrastructure-AppDev
      type: git
      name: EDR-Infrastructure-AppDev
      ref: master
    - repository: EDR-Infrastructure-ConfigMGMT
      type: git
      name: EDR-Infrastructure-ConfigMGMT
      ref: master
    - repository: EDR-Infrastructure-Environments
      type: git
      name: EDR-Infrastructure-Environments
      ref: master
    - repository: EDR-Infrastructure-Hive
      type: git
      name: EDR-Infrastructure-Hive
      ref: master
    - repository: EDR-Infrastructure-PRPC
      type: git
      name: EDR-Infrastructure-PRPC
      ref: master
    - repository: EDR-Invariant-DataTools
      type: git
      name: EDR-Invariant-DataTools
      ref: master
    - repository: EDR-Invariant-Legacy-Archive
      type: git
      name: EDR-Invariant-Legacy-Archive
      ref: master
    - repository: EDR-Invariant-Legacy-Conversion
      type: git
      name: EDR-Invariant-Legacy-Conversion
      ref: master
    - repository: IVR-Mindful-CallBack
      type: git
      name: IVR Mindful CallBack
      ref: master
    - repository: EDR-Knowledge-Library
      type: git
      name: EDR-Knowledge-Library
      ref: master
    - repository: EDR-Message-Repeater-Demographics
      type: git
      name: EDR-Message-Repeater-Demographics
      ref: master
    - repository: EDR-MyFTB-Fillable-Forms
      type: git
      name: EDR-MyFTB-Fillable-Forms
      ref: master
    - repository: EDR-MyFTB-Services
      type: git
      name: EDR-MyFTB-Services
      ref: master
    - repository: EDR-Non-Prod-Utilities
      type: git
      name: EDR-Non-Prod-Utilities
      ref: master
    - repository: EDR-Offer-In-Compromise-Service
      type: git
      name: EDR-Offer-In-Compromise-Service
      ref: master
    - repository: EDR-Offer-In-Compromise-UI
      type: git
      name: EDR-Offer-In-Compromise-UI
      ref: master
    - repository: EDR-Online-Help
      type: git
      name: EDR-Online-Help
      ref: master
    - repository: EDR-Open-Case-Doc
      type: git
      name: EDR-Open-Case-Doc
      ref: master
    - repository: EDR-Ops-Monitoring-Service
      type: git
      name: EDR-Ops-Monitoring-Service
      ref: master
    - repository: EDR-PDF-Services
      type: git
      name: EDR-PDF-Services
      ref: master
    - repository: EDR-Persistence-EOD
      type: git
      name: EDR-Persistence-EOD
      ref: master
    - repository: EDR-Preferences-Services
      type: git
      name: EDR-Preferences-Services
      ref: master
    - repository: EDR-Preferences-UI
      type: git
      name: EDR-Preferences-UI
      ref: master
    - repository: EDR-Real-Estate-Withholding-Return-UI
      type: git
      name: EDR-Real-Estate-Withholding-Return-UI
      ref: master
    - repository: EDR-Relationships-Services
      type: git
      name: EDR-Relationships-Services
      ref: master
    - repository: EDR-Representatives-Services
      type: git
      name: EDR-Representatives-Services
      ref: master
    - repository: EDR-Representatives-UI
      type: git
      name: EDR-Representatives-UI
      ref: master
    - repository: EDR-Returns-Filing-Services
      type: git
      name: EDR-Returns-Filing-Services
      ref: master
    - repository: EDR-Returns-Filing-UI
      type: git
      name: EDR-Returns-Filing-UI
      ref: master
    - repository: EDR-Sanctum
      type: git
      name: EDR-Sanctum
      ref: master
    - repository: EDR-ThirdParty-Services
      type: git
      name: EDR-ThirdParty-Services
      ref: master
    - repository: EDR-ThirdParty-UI
      type: git
      name: EDR-ThirdParty-UI
      ref: master
    - repository: EDR-TPF-UI
      type: git
      name: EDR-TPF-UI
      ref: master
    - repository: EDR-Withholding-Return-Batch
      type: git
      name: EDR-Withholding-Return-Batch
      ref: master
    - repository: EDR-Withholding-Return-Persistence
      type: git
      name: EDR-Withholding-Return-Persistence
      ref: master
    - repository: EPSS-Python-Training
      type: git
      name: EPSS-Python-Training
      ref: master
    - repository: ETS-Environment-Properties
      type: git
      name: ETS-Environment-Properties
      ref: master
    - repository: Modular-App-POC
      type: git
      name: Modular-App-POC
      ref: master
    - repository: PA-COMM-MGMT
      type: git
      name: PA-COMM-MGMT
      ref: master
    - repository: FH-SSO-POC
      type: git
      name: FH-SSO-POC
      ref: master
    - repository: TfsReporting
      type: git
      name: TfsReporting
      ref: master
    - repository: Third-Party-Data
      type: git
      name: Third-Party-Data
      ref: master

pool:
  name: 'Java-Maven'

steps:
  # Check out all repos (master)
  - checkout: Arisant
    clean: true
  - checkout: EDL-Utilities
    clean: true
  - checkout: EDR-AEM-Utilities
    clean: true
  - checkout: EDR-AMZ-Utilities
    clean: true
  - checkout: EDR-AnalyticModels-Audit
    clean: true
  - checkout: EDR-AnalyticModels-Collections
    clean: true
  - checkout: EDR-AnalyticModels-FE
    clean: true
  - checkout: EDR-AnalyticModels-Legal
    clean: true
  - checkout: EDR-AnalyticModels-Pipelines
    clean: true
  - checkout: EDR-AnalyticModels-RA
    clean: true
  - checkout: EDR-AppDev-Forms
    clean: true
  - checkout: EDR-AppDev-Middleware
    clean: true
  - checkout: EDR-AppDev-NonJava
    clean: true
  - checkout: EDR-Architecture-Sample
    clean: true
  - checkout: EDR-Automation-Test
    clean: true
  - checkout: EDR-Batch-Client
    clean: true
  - checkout: EDR-Case-Archive
    clean: true
  - checkout: EDR-Case-Document-API
    clean: true
  - checkout: EDR-Case-Document-Templates
    clean: true
  - checkout: EDR-CnfgMgmt-Ansible
    clean: true
  - checkout: EDR-CnfgMgmt-Pipelines
    clean: true
  - checkout: EDR-Collections-Batch
    clean: true
  - checkout: EDR-Collections-Integration
    clean: true
  - checkout: EDR-Collections-Persistence
    clean: true
  - checkout: EDR-Data-ETL
    clean: true
  - checkout: EDR-Data-MDM
    clean: true
  - checkout: EDR-Data-PySpark
    clean: true
  - checkout: EDR-Data-Virtualization
    clean: true
  - checkout: EDR-Data-Visualization
    clean: true
  - checkout: EDR-EASE-Okta-MyFTB-Integration
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
  - checkout: EDR-Health-Checks-Dashboard
    clean: true
  - checkout: EDR-Hearing-Services
    clean: true
  - checkout: EDR-iCapture
    clean: true
  - checkout: EDR-Infrastructure-AppDev
    clean: true
  - checkout: EDR-Infrastructure-ConfigMGMT
    clean: true
  - checkout: EDR-Infrastructure-Environments
    clean: true
  - checkout: EDR-Infrastructure-Hive
    clean: true
  - checkout: EDR-Infrastructure-PRPC
    clean: true
  - checkout: EDR-Invariant-DataTools
    clean: true
  - checkout: EDR-Invariant-Legacy-Archive
    clean: true
  - checkout: EDR-Invariant-Legacy-Conversion
    clean: true
  - checkout: IVR-Mindful-CallBack
    clean: true
  - checkout: EDR-Knowledge-Library
    clean: true
  - checkout: EDR-Message-Repeater-Demographics
    clean: true
  - checkout: EDR-MyFTB-Fillable-Forms
    clean: true
  - checkout: EDR-MyFTB-Services
    clean: true
  - checkout: EDR-Non-Prod-Utilities
    clean: true
  - checkout: EDR-Offer-In-Compromise-Service
    clean: true
  - checkout: EDR-Offer-In-Compromise-UI
    clean: true
  - checkout: EDR-Online-Help
    clean: true
  - checkout: EDR-Open-Case-Doc
    clean: true
  - checkout: EDR-Ops-Monitoring-Service
    clean: true
  - checkout: EDR-PDF-Services
    clean: true
  - checkout: EDR-Persistence-EOD
    clean: true
  - checkout: EDR-Preferences-Services
    clean: true
  - checkout: EDR-Preferences-UI
    clean: true
  - checkout: EDR-Real-Estate-Withholding-Return-UI
    clean: true
  - checkout: EDR-Relationships-Services
    clean: true
  - checkout: EDR-Representatives-Services
    clean: true
  - checkout: EDR-Representatives-UI
    clean: true
  - checkout: EDR-Returns-Filing-Services
    clean: true
  - checkout: EDR-Returns-Filing-UI
    clean: true
  - checkout: EDR-Sanctum
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
  - checkout: EPSS-Python-Training
    clean: true
  - checkout: ETS-Environment-Properties
    clean: true
  - checkout: Modular-App-POC
    clean: true
  - checkout: PA-COMM-MGMT
    clean: true
  - checkout: FH-SSO-POC
    clean: true
  - checkout: TfsReporting
    clean: true
  - checkout: Third-Party-Data
    clean: true

  # One-time Java 17 setup
  - task: JavaToolInstaller@0
    displayName: 'Use Java 17'
    inputs:
      versionSpec: 17
      jdkArchitectureOption: x64
      jdkSourceOption: PreInstalled

  # Single Nexus IQ scan over the entire workspace
  - task: SonatypeIntegrations.nexus-iq-azure-extension.nexus-iq-azure-pipeline-task.NexusIqPipelineTask@2
    displayName: 'Nexus IQ Scan (All repos)'
    inputs:
      nexusIqService: 'Nexus IQ Server'
      applicationId: 'EDR1_Repos_Pipeline'
      stage: build
      scanTargets: '**/* !**/node_modules/** !**/*.js !**/*.css !**/*.json !**/*.map'
      scanPipelineWorkspace: true
