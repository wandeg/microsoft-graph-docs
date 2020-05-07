---
title: "Enum values"
description: "Microsoft Graph enumeration values"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: enumTypes
---

### actionState values 


State of the action on the device

|Members|
|:---|
|none|
|pending|
|canceled|
|active|
|done|
|failed|
|notSupported|

### adminConsentState values 

Admin consent state.

|Members|
|:---|
|notConfigured|
|granted|
|notGranted|

### appLogDecryptionAlgorithm values 

**TODO: Add Description**

|Members|
|:---|
|aes256|

### appLogUploadState values 

AppLogUploadStatus

|Members|
|:---|
|pending|
|completed|
|failed|

### chassisType values 

Chassis type.

|Members|
|:---|
|unknown|
|desktop|
|laptop|
|worksWorkstation|
|enterpriseServer|
|phone|
|tablet|
|mobileOther|
|mobileUnknown|

### coManagementEligibleType values 

**TODO: Add Description**

|Members|
|:---|
|coManaged|
|eligible|
|eligibleButNotAadJoined|
|needsOSUpdate|

### complianceState values 

Compliance state.

|Members|
|:---|
|unknown|
|compliant|
|noncompliant|
|conflict|
|error|
|inGracePeriod|
|configManager|

### configurationManagerActionDeliveryStatus values 

Delivery state of Configuration Manager device action

|Members|
|:---|
|unknown|
|pendingDelivery|
|deliveredToConnectorService|
|failedToDeliverToConnectorService|
|deliveredToOnPremisesServer|

### configurationManagerActionType values 

Action type on Configuration Manager client

|Members|
|:---|
|refreshMachinePolicy|
|refreshUserPolicy|
|wakeUpClient|
|appEvaluation|

### configurationManagerClientState values 

Configuration manager client state

|Members|
|:---|
|unknown|
|installed|
|healthy|
|installFailed|
|updateFailed|
|communicationError|

### deviceEnrollmentType values 

Possible ways of adding a mobile device to management.

|Members|
|:---|
|unknown|
|userEnrollment|
|deviceEnrollmentManager|
|appleBulkWithUser|
|appleBulkWithoutUser|
|windowsAzureADJoin|
|windowsBulkUserless|
|windowsAutoEnrollment|
|windowsBulkAzureDomainJoin|
|windowsCoManagement|
|appleUserEnrollment|
|appleUserEnrollmentWithServiceAccount|
|azureAdJoinUsingAzureVmExtension|

### deviceGuardLocalSystemAuthorityCredentialGuardState values 

**TODO: Add Description**

|Members|
|:---|
|running|
|rebootRequired|
|notLicensed|
|notConfigured|
|virtualizationBasedSecurityNotRunning|

### deviceGuardVirtualizationBasedSecurityHardwareRequirementState values 

**TODO: Add Description**

|Members|
|:---|
|meetHardwareRequirements|
|secureBootRequired|
|dmaProtectionRequired|
|hyperVNotSupportedForGuestVM|
|hyperVNotAvailable|

### deviceGuardVirtualizationBasedSecurityState values 

**TODO: Add Description**

|Members|
|:---|
|running|
|rebootRequired|
|require64BitArchitecture|
|notLicensed|
|notConfigured|
|doesNotMeetHardwareRequirements|
|other|

### deviceManagementExchangeAccessState values 

Device Exchange Access State.

|Members|
|:---|
|none|
|unknown|
|allowed|
|blocked|
|quarantined|

### deviceManagementExchangeAccessStateReason values 

Device Exchange Access State Reason.

|Members|
|:---|
|none|
|unknown|
|exchangeGlobalRule|
|exchangeIndividualRule|
|exchangeDeviceRule|
|exchangeUpgrade|
|exchangeMailboxPolicy|
|other|
|compliant|
|notCompliant|
|notEnrolled|
|unknownLocation|
|mfaRequired|
|azureADBlockDueToAccessPolicy|
|compromisedPassword|
|deviceNotKnownWithManagedApp|

### deviceManagementSubscriptions values 

Tenant mobile device management subscriptions.

|Members|
|:---|
|none|
|intune|
|office365|
|intunePremium|
|intune_EDU|
|intune_SMB|

### deviceManagementSubscriptionState values 

Tenant mobile device management subscription state.

|Members|
|:---|
|pending|
|active|
|warning|
|disabled|
|deleted|
|blocked|
|lockedOut|

### deviceRegistrationState values 

Device registration status.

|Members|
|:---|
|notRegistered|
|registered|
|revoked|
|keyConflict|
|approvalPending|
|certificateReset|
|notRegisteredPendingEnrollment|
|unknown|

### deviceType values 

Device type.

|Members|
|:---|
|desktop|
|windowsRT|
|winMO6|
|nokia|
|windowsPhone|
|mac|
|winCE|
|winEmbedded|
|iPhone|
|iPad|
|iPod|
|android|
|iSocConsumer|
|unix|
|macMDM|
|holoLens|
|surfaceHub|
|androidForWork|
|androidEnterprise|
|windows10x|
|blackberry|
|palm|
|unknown|

### diskType values 

**TODO: Add Description**

|Members|
|:---|
|unkown|
|hdd|
|ssd|

### globalDeviceHealthScriptState values 

Indicates whether global device health scripts are enabled and are in which state

|Members|
|:---|
|notConfigured|
|pending|
|enabled|

### healthState values 

Indicates health state of the Windows management app.

|Members|
|:---|
|unknown|
|healthy|
|unhealthy|

### lostModeState values 

State of lost mode, indicating if lost mode is enabled or disabled

|Members|
|:---|
|disabled|
|enabled|

### managedDeviceArchitecture values 

Processor architecture

|Members|
|:---|
|unknown|
|x86|
|x64|
|arm|
|arM64|

### managedDeviceOwnerType values 

Owner type of device.

|Members|
|:---|
|unknown|
|company|
|personal|

### managedDevicePartnerReportedHealthState values 

Available health states for the Device Health API

|Members|
|:---|
|unknown|
|activated|
|deactivated|
|secured|
|lowSeverity|
|mediumSeverity|
|highSeverity|
|unresponsive|
|compromised|
|misconfigured|

### managedDeviceRemoteAction values 

**TODO: Add Description**

|Members|
|:---|
|retire|
|delete|
|fullScan|
|quickScan|
|signatureUpdate|
|wipe|
|customTextNotification|
|rebootNow|
|setDeviceName|

### managementAgentType values 

Management agent type.

|Members|
|:---|
|eas|
|mdm|
|easMdm|
|intuneClient|
|easIntuneClient|
|configurationManagerClient|
|configurationManagerClientMdm|
|configurationManagerClientMdmEas|
|unknown|
|jamf|
|googleCloudDevicePolicyController|
|microsoft365ManagedMdm|
|windowsManagementCloudApi|

### managementState values 

Management state of device in Microsoft Intune.

|Members|
|:---|
|managed|
|retirePending|
|retireFailed|
|wipePending|
|wipeFailed|
|unhealthy|
|deletePending|
|retireIssued|
|wipeIssued|
|wipeCanceled|
|retireCanceled|
|discovered|

### ownerType values 

Owner type of device.

|Members|
|:---|
|unknown|
|company|
|personal|

### remediationState values 

Indicates the type of execution status of the device management script.

|Members|
|:---|
|unknown|
|skipped|
|success|
|remediationFailed|
|scriptError|

### remoteAction values 

Remote actions Intune supports.

|Members|
|:---|
|unknown|
|factoryReset|
|removeCompanyData|
|resetPasscode|
|remoteLock|
|enableLostMode|
|disableLostMode|
|locateDevice|
|rebootNow|
|recoverPasscode|
|cleanWindowsDevice|
|logoutSharedAppleDeviceActiveUser|
|quickScan|
|fullScan|
|windowsDefenderUpdateSignatures|
|factoryResetKeepEnrollmentData|
|updateDeviceAccount|
|automaticRedeployment|
|shutDown|
|rotateBitLockerKeys|
|rotateFileVaultKey|
|getFileVaultKey|
|setDeviceName|

### runAsAccountType values 

Indicates the type of execution context the device management script runs in.

|Members|
|:---|
|system|
|user|

### runState values 

Indicates the type of execution status of the device management script.

|Members|
|:---|
|unknown|
|success|
|fail|
|scriptError|
|pending|
|notApplicable|

### userExperienceAnalyticsHealthState values 

**TODO: Add Description**

|Members|
|:---|
|unknown|
|insufficientData|
|needsAttention|
|meetingGoals|

### userExperienceAnalyticsInsightSeverity values 

**TODO: Add Description**

|Members|
|:---|
|none|
|informational|
|warning|
|error|

### userExperienceAnalyticsSummarizedBy values 

**TODO: Add Description**

|Members|
|:---|
|none|
|model|
|allRegressions|
|modelRegression|
|manufacturerRegression|
|operatingSystemVersionRegression|

### windowsDeviceHealthState values 

Computer endpoint protection state

|Members|
|:---|
|clean|
|fullScanPending|
|rebootPending|
|manualStepsPending|
|offlineScanPending|
|critical|

### windowsMalwareCategory values 

Malware category id

|Members|
|:---|
|invalid|
|adware|
|spyware|
|passwordStealer|
|trojanDownloader|
|worm|
|backdoor|
|remoteAccessTrojan|
|trojan|
|emailFlooder|
|keylogger|
|dialer|
|monitoringSoftware|
|browserModifier|
|cookie|
|browserPlugin|
|aolExploit|
|nuker|
|securityDisabler|
|jokeProgram|
|hostileActiveXControl|
|softwareBundler|
|stealthNotifier|
|settingsModifier|
|toolBar|
|remoteControlSoftware|
|trojanFtp|
|potentialUnwantedSoftware|
|icqExploit|
|trojanTelnet|
|exploit|
|filesharingProgram|
|malwareCreationTool|
|remote_Control_Software|
|tool|
|trojanDenialOfService|
|trojanDropper|
|trojanMassMailer|
|trojanMonitoringSoftware|
|trojanProxyServer|
|virus|
|known|
|unknown|
|spp|
|behavior|
|vulnerability|
|policy|
|enterpriseUnwantedSoftware|
|ransom|
|hipsRule|

### windowsMalwareExecutionState values 

Malware execution status

|Members|
|:---|
|unknown|
|blocked|
|allowed|
|running|
|notRunning|

### windowsMalwareSeverity values 

Malware severity

|Members|
|:---|
|unknown|
|low|
|moderate|
|high|
|severe|

### windowsMalwareState values 

Malware current status

|Members|
|:---|
|unknown|
|detected|
|cleaned|
|quarantined|
|removed|
|allowed|
|blocked|
|cleanFailed|
|quarantineFailed|
|removeFailed|
|allowFailed|
|abandoned|
|blockFailed|

### windowsMalwareThreatState values 

Malware threat status

|Members|
|:---|
|active|
|actionFailed|
|manualStepsRequired|
|fullScanRequired|
|rebootRequired|
|remediatedWithNonCriticalFailures|
|quarantined|
|removed|
|cleaned|
|allowed|
|noStatusCleared|

