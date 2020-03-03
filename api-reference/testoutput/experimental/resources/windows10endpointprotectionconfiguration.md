---
title: "windows10EndpointProtectionConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the Windows10EndpointProtectionConfiguration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windows10EndpointProtectionConfiguration resource type

This topic provides descriptions of the declared methods, properties and relationships exposed by the Windows10EndpointProtectionConfiguration resource.


Inherits from [deviceConfiguration](../resources/deviceConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windows10EndpointProtectionConfigurations](../api/windows10endpointprotectionconfiguration-list.md)|[windows10EndpointProtectionConfiguration](../resources/windows10EndpointProtectionConfiguration.md) collection|List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) objects.|
|[Get windows10EndpointProtectionConfiguration](../api/windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/windows10EndpointProtectionConfiguration.md)|Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) object.|
|[Create windows10EndpointProtectionConfiguration](../api/windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/windows10EndpointProtectionConfiguration.md)|Create a new [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) object.|
|[Delete windows10EndpointProtectionConfiguration](../api/windows10endpointprotectionconfiguration-delete.md)|None|Deletes a [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md).|
|[Update windows10EndpointProtectionConfiguration](../api/windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/windows10EndpointProtectionConfiguration.md)|Update the properties of a [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) object.|
|[assign](../api/windows10endpointprotectionconfiguration-assign.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection||
|[windowsPrivacyAccessControls](../api/windows10endpointprotectionconfiguration-windowsprivacyaccesscontrols.md)|None||
|[assignedAccessMultiModeProfiles](../api/windows10endpointprotectionconfiguration-assignedaccessmultimodeprofiles.md)|None||
|[List groupAssignments](../api/windows10endpointprotectionconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/windows10endpointprotectionconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/windows10endpointprotectionconfiguration-list-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|Get the deviceConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/windows10endpointprotectionconfiguration-post-assignments.md)|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/windows10endpointprotectionconfiguration-list-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/windows10endpointprotectionconfiguration-post-devicestatuses.md)|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/windows10endpointprotectionconfiguration-list-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/windows10endpointprotectionconfiguration-post-userstatuses.md)|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get deviceConfigurationDeviceOverview](../api/deviceconfigurationdeviceoverview-get.md)|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/deviceconfigurationuseroverview-get.md)|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/deviceconfigurationuseroverview.md) object.|
|[List deviceSettingStateSummaries](../api/windows10endpointprotectionconfiguration-list-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Get the settingStateDeviceSummaries from the deviceSettingStateSummaries navigation property.|
|[Add deviceSettingStateSummaries](../api/windows10endpointprotectionconfiguration-post-devicesettingstatesummaries.md)|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md)|Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationGuardAllowFileSaveOnHost|Boolean|Allow users to download files from Edge in the application guard container and save them on the host file system|
|applicationGuardAllowPersistence|Boolean|Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Allow printing to Local Printers from Container|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Allow printing to Network Printers from Container|
|applicationGuardAllowPrintToPDF|Boolean|Allow printing to PDF from Container|
|applicationGuardAllowPrintToXPS|Boolean|Allow printing to XPS from Container|
|applicationGuardAllowVirtualGPU|Boolean|Allow application guard to use virtual GPU|
|applicationGuardBlockClipboardSharing|Enumeration|Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways. Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardBlockFileTransfer|Enumeration|Block clipboard to transfer image file, text file or neither of them. Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Block enterprise sites to load non-enterprise content, such as third party plug-ins|
|applicationGuardEnabled|Boolean|Enable Windows Defender Application Guard|
|applicationGuardEnabledOptions|Enumeration|Enable Windows Defender Application Guard for newer Windows builds. Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardForceAuditing|Boolean|Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)|
|appLockerApplicationControl|Enumeration|Enables the Admin to choose what types of app to allow on devices. Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|bitLockerAllowStandardUserEncryption|Boolean|Allows the admin to allow standard users to enable encrpytion during Azure AD Join.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Allows the Admin to disable the warning prompt for other disk encryption on the user machines.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Allows the admin to require encryption to be turned on using BitLocker. This policy is valid only for a mobile SKU.|
|bitLockerEncryptDevice|Boolean|Allows the admin to require encryption to be turned on using BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/bitLockerFixedDrivePolicy.md)|BitLocker Fixed Drive Policy.|
|bitLockerRecoveryPasswordRotation|Enumeration|This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE). Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/bitLockerRemovableDrivePolicy.md)|BitLocker Removable Drive Policy.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/bitLockerSystemDrivePolicy.md)|BitLocker System Drive Policy.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|defenderAdditionalGuardedFolders|String collection|List of folder paths to be added to the list of protected folders|
|defenderAdobeReaderLaunchChildProcess|Enumeration|Value indicating the behavior of Adobe Reader from creating child processes. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderAdvancedRansomewareProtectionType|Enumeration|Value indicating use of advanced protection against ransomeware. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderAttackSurfaceReductionExcludedPaths|String collection|List of exe files and folders to be excluded from attack surface reduction rules|
|defenderBlockEndUserAccess|Boolean|Allows or disallows user access to the Windows Defender UI. If disallowed, all Windows Defender notifications will also be suppressed.|
|defenderCheckForSignaturesBeforeRunningScan|Boolean|This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.|
|defenderCloudBlockLevel|Enumeration|Added in Windows 10, version 1709. This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files. Value type is integer. This feature requires the "Join Microsoft MAPS" setting enabled in order to function. Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeoutInSeconds|Int32|Added in Windows 10, version 1709. This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe. Value type is integer, range is 0 - 50. This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required". Valid values 0 to 50|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Time period (in days) that quarantine items will be stored on the system. Valid values 0 to 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/defenderDetectedMalwareActions.md)|Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.|
|defenderDisableBehaviorMonitoring|Boolean|Allows or disallows Windows Defender Behavior Monitoring functionality.|
|defenderDisableCatchupFullScan|Boolean|This policy setting allows you to configure catch-up scans for scheduled full scans. A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed. Usually these scheduled scans are missed because the computer was turned off at the scheduled time.|
|defenderDisableCatchupQuickScan|Boolean|This policy setting allows you to configure catch-up scans for scheduled quick scans. A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed. Usually these scheduled scans are missed because the computer was turned off at the scheduled time.|
|defenderDisableCloudProtection|Boolean|To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds. Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.|
|defenderDisableIntrusionPreventionSystem|Boolean|Allows or disallows Windows Defender Intrusion Prevention functionality.|
|defenderDisableOnAccessProtection|Boolean|Allows or disallows Windows Defender On Access Protection functionality.|
|defenderDisableRealTimeMonitoring|Boolean|Allows or disallows Windows Defender Realtime Monitoring functionality.|
|defenderDisableScanArchiveFiles|Boolean|Allows or disallows scanning of archives.|
|defenderDisableScanDownloads|Boolean|Allows or disallows Windows Defender IOAVP Protection functionality.|
|defenderDisableScanNetworkFiles|Boolean|Allows or disallows a scanning of network files.|
|defenderDisableScanRemovableDrivesDuringFullScan|Boolean|Allows or disallows a full scan of removable drives. During a quick scan, removable drives may still be scanned.|
|defenderDisableScanScriptsLoadedInInternetExplorer|Boolean|Allows or disallows Windows Defender Script Scanning functionality.|
|defenderEmailContentExecution|Enumeration|Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client). Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderEmailContentExecutionType|Enumeration|Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client). Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderEnableLowCpuPriority|Boolean|This policy setting allows you to enable or disable low CPU priority for scheduled scans.|
|defenderEnableScanIncomingMail|Boolean|Allows or disallows scanning of email.|
|defenderEnableScanMappedNetworkDrivesDuringFullScan|Boolean|Allows or disallows a full scan of mapped network drives.|
|defenderExploitProtectionXml|Binary|Xml content containing information regarding exploit protection details.|
|defenderExploitProtectionXmlFileName|String|Name of the file from which DefenderExploitProtectionXml was obtained.|
|defenderFileExtensionsToExclude|String collection|File extensions to exclude from scans and real time protection.|
|defenderFilesAndFoldersToExclude|String collection|Files and folder to exclude from scans and real time protection.|
|defenderGuardedFoldersAllowedAppPaths|String collection|List of paths to exe that are allowed to access protected folders|
|defenderGuardMyFoldersType|Enumeration|Value indicating the behavior of protected folders. Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderNetworkProtectionType|Enumeration|Value indicating the behavior of NetworkProtection. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunch|Enumeration|Value indicating the behavior of Office applications/macros creating or launching executable content. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsExecutableContentCreationOrLaunchType|Enumeration|Value indicating the behavior of Office applications/macros creating or launching executable content. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderOfficeAppsLaunchChildProcess|Enumeration|Value indicating the behavior of Office application launching child processes. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsLaunchChildProcessType|Enumeration|Value indicating the behavior of Office application launching child processes. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderOfficeAppsOtherProcessInjection|Enumeration|Value indicating the behavior of  Office applications injecting into other processes. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeAppsOtherProcessInjectionType|Enumeration|Value indicating the behavior of Office applications injecting into other processes. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderOfficeCommunicationAppsLaunchChildProcess|Enumeration|Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32Imports|Enumeration|Value indicating the behavior of Win32 imports from Macro code in Office. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|Enumeration|Value indicating the behavior of Win32 imports from Macro code in Office. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderPotentiallyUnwantedAppAction|Enumeration|Added in Windows 10, version 1607. Specifies the level of detection for potentially unwanted applications (PUAs). Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderPreventCredentialStealingType|Enumeration|Value indicating if credential stealing from the Windows local security authority subsystem is permitted. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderProcessCreation|Enumeration|Value indicating response to process creations originating from PSExec and WMI commands. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderProcessCreationType|Enumeration|Value indicating response to process creations originating from PSExec and WMI commands. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderProcessesToExclude|String collection|Processes to exclude from scans and real time protection.|
|defenderScanDirection|Enumeration|Controls which sets of files should be monitored. Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderScanMaxCpuPercentage|Int32|Represents the average CPU load factor for the Windows Defender scan (in percent). The default value is 50. Valid values 0 to 100|
|defenderScanType|Enumeration|Selects whether to perform a quick scan or full scan. Possible values are: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|Selects the time of day that the Windows Defender quick scan should run. For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM. The default value is 120|
|defenderScheduledScanDay|Enumeration|Selects the day that the Windows Defender scan should run. Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Selects the time of day that the Windows Defender scan should run.|
|defenderScriptDownloadedPayloadExecution|Enumeration|Value indicating the behavior of js/vbs executing payload downloaded from Internet. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderScriptDownloadedPayloadExecutionType|Enumeration|Value indicating the behavior of js/vbs executing payload downloaded from Internet. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderScriptObfuscatedMacroCode|Enumeration|Value indicating the behavior of obfuscated js/vbs/ps/macro code. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderScriptObfuscatedMacroCodeType|Enumeration|Value indicating the behavior of obfuscated js/vbs/ps/macro code. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Indicates whether or not to block user from overriding Exploit Protection settings.|
|defenderSecurityCenterDisableAccountUI|Boolean|Used to disable the display of the account protection area.|
|defenderSecurityCenterDisableAppBrowserUI|Boolean|Used to disable the display of the app and browser protection area.|
|defenderSecurityCenterDisableClearTpmUI|Boolean|Used to disable the display of the Clear TPM button.|
|defenderSecurityCenterDisableFamilyUI|Boolean|Used to disable the display of the family options area.|
|defenderSecurityCenterDisableHardwareUI|Boolean|Used to disable the display of the hardware protection area.|
|defenderSecurityCenterDisableHealthUI|Boolean|Used to disable the display of the device performance and health area.|
|defenderSecurityCenterDisableNetworkUI|Boolean|Used to disable the display of the firewall and network protection area.|
|defenderSecurityCenterDisableNotificationAreaUI|Boolean|Used to disable the display of the notification area control. The user needs to either sign out and sign in or reboot the computer for this setting to take effect.|
|defenderSecurityCenterDisableRansomwareUI|Boolean|Used to disable the display of the ransomware protection area. |
|defenderSecurityCenterDisableSecureBootUI|Boolean|Used to disable the display of the secure boot area under Device security.|
|defenderSecurityCenterDisableTroubleshootingUI|Boolean|Used to disable the display of the security process troubleshooting under Device security.|
|defenderSecurityCenterDisableVirusUI|Boolean|Used to disable the display of the virus and threat protection area.|
|defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI|Boolean|Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.|
|defenderSecurityCenterHelpEmail|String|The email address that is displayed to users.|
|defenderSecurityCenterHelpPhone|String|The phone number or Skype ID that is displayed to users.|
|defenderSecurityCenterHelpURL|String|The help portal URL this is displayed to users.|
|defenderSecurityCenterITContactDisplay|Enumeration|Configure where to display IT contact information to end users. Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|defenderSecurityCenterNotificationsFromApp|Enumeration|Notifications to show from the displayed areas of app. Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|defenderSecurityCenterOrganizationDisplayName|String|The company name that is displayed to the users.|
|defenderSubmitSamplesConsentType|Enumeration|Checks for the user consent level in Windows Defender to send data. Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderUntrustedExecutable|Enumeration|Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderUntrustedExecutableType|Enumeration|Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria. Possible values are: `userDefined`, `block`, `auditMode`.|
|defenderUntrustedUSBProcess|Enumeration|Value indicating response to untrusted and unsigned processes that run from USB. Possible values are: `userDefined`, `enable`, `auditMode`.|
|defenderUntrustedUSBProcessType|Enumeration|Value indicating response to untrusted and unsigned processes that run from USB. Possible values are: `userDefined`, `block`, `auditMode`.|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceGuardEnableSecureBootWithDMA|Boolean|This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA. Specifies whether Platform Security Level is enabled at next reboot.|
|deviceGuardEnableVirtualizationBasedSecurity|Boolean|Turns On Virtualization Based Security(VBS).|
|deviceGuardLaunchSystemGuard|Enumeration|Allows the IT admin to configure the launch of System Guard. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|deviceGuardLocalSystemAuthorityCredentialGuardSettings|Enumeration|Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled. Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.|
|deviceGuardSecureBootWithDMA|Enumeration|Specifies whether Platform Security Level is enabled at next reboot. Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/deviceManagementApplicabilityRuleDeviceMode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/deviceManagementApplicabilityRuleOsEdition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/deviceManagementApplicabilityRuleOsVersion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|dmaGuardDeviceEnumerationPolicy|Enumeration|This policy is intended to provide additional security against external DMA capable devices. It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing. This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware. Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user. It has to be supported by the system at the time of manufacturing. To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe. Possible values are: `deviceDefault`, `blockAll`, `allowAll`.|
|firewallBlockStatefulFTP|Boolean|Blocks stateful FTP connections to the device|
|firewallCertificateRevocationListCheckMethod|Enumeration|Specify how the certificate revocation list is to be enforced. Possible values are: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive. This is the period after which security associations will expire and be deleted. Valid values 300 to 3600|
|firewallIPSecExemptionsAllowDHCP|Boolean|Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic|
|firewallIPSecExemptionsAllowICMP|Boolean|Configures IPSec exemptions to allow ICMP|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes|
|firewallMergeKeyingModuleSettings|Boolean|If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set|
|firewallPacketQueueingMethod|Enumeration|Configures how packet queueing should be applied in the tunnel gateway scenario. Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallPreSharedKeyEncodingMethod|Enumeration|Select the preshared key encoding to be used. Possible values are: `deviceDefault`, `none`, `utF8`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/windowsFirewallNetworkProfile.md)|Configures the firewall profile settings for domain networks|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/windowsFirewallNetworkProfile.md)|Configures the firewall profile settings for private networks|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/windowsFirewallNetworkProfile.md)|Configures the firewall profile settings for public networks|
|firewallRules|[windowsFirewallRule](../resources/windowsFirewallRule.md) collection|Configures the firewall rule settings. This collection can contain a maximum of 150 elements.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lanManagerAuthenticationLevel|Enumeration|This security setting determines which challenge/response authentication protocol is used for network logons. Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|lanManagerWorkstationDisableInsecureGuestLogons|Boolean|If enabled,the SMB client will allow insecure guest logons. If not configured, the SMB client will reject insecure guest logons.|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|localSecurityOptionsAdministratorAccountName|String|Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.|
|localSecurityOptionsAdministratorElevationPromptBehavior|Enumeration|Define the behavior of the elevation prompt for admins in Admin Approval Mode. Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares|Boolean|This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Boolean|Block PKU2U authentication requests to this device to use online identities.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager|String|Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.|
|localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool|Boolean|UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity|
|localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn|Boolean|This security setting determines whether a computer can be shut down without having to log on to Windows.|
|localSecurityOptionsAllowUIAccessApplicationElevation|Boolean|Allow UIAccess apps to prompt for elevation without using the secure desktop.|
|localSecurityOptionsAllowUIAccessApplicationsForSecureLocations|Boolean|Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled|
|localSecurityOptionsAllowUndockWithoutHavingToLogon|Boolean|Prevent a portable computer from being undocked without having to log in.|
|localSecurityOptionsBlockMicrosoftAccounts|Boolean|Prevent users from adding new Microsoft accounts to this computer.|
|localSecurityOptionsBlockRemoteLogonWithBlankPassword|Boolean|Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled|
|localSecurityOptionsBlockRemoteOpticalDriveAccess|Boolean|Enabling this settings allows only interactively logged on user to access CD-ROM media.|
|localSecurityOptionsBlockUsersInstallingPrinterDrivers|Boolean|Restrict installing printer drivers as part of connecting to a shared printer to admins only.|
|localSecurityOptionsClearVirtualMemoryPageFile|Boolean|This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.|
|localSecurityOptionsClientDigitallySignCommunicationsAlways|Boolean|This security setting determines whether packet signing is required by the SMB client component.|
|localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers|Boolean|If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.|
|localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation|Boolean|App installations requiring elevated privileges will prompt for admin credentials.Default is enabled|
|localSecurityOptionsDisableAdministratorAccount|Boolean|Determines whether the Local Administrator account is enabled or disabled.|
|localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees|Boolean|This security setting determines whether the SMB client attempts to negotiate SMB packet signing.|
|localSecurityOptionsDisableGuestAccount|Boolean|Determines if the Guest account is enabled or disabled.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsAlways|Boolean|This security setting determines whether packet signing is required by the SMB server component.|
|localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees|Boolean|This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.|
|localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts|Boolean|This security setting determines what additional permissions will be granted for anonymous connections to the computer.|
|localSecurityOptionsDoNotRequireCtrlAltDel|Boolean|Require CTRL+ALT+DEL to be pressed before a user can log on.|
|localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange|Boolean|This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored. It’s not stored by default.|
|localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser|Enumeration|Define who is allowed to format and eject removable NTFS media. Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsGuestAccountName|String|Define a different account name to be associated with the security identifier (SID) for the account “Guest”.|
|localSecurityOptionsHideLastSignedInUser|Boolean|Do not display the username of the last person who signed in on this device.|
|localSecurityOptionsHideUsernameAtSignIn|Boolean|Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.|
|localSecurityOptionsInformationDisplayedOnLockScreen|Enumeration|Configure the user information that is displayed when the session is locked. If not configured, user display name, domain and username are shown. Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|localSecurityOptionsInformationShownOnLockScreen|Enumeration|Configure the user information that is displayed when the session is locked. If not configured, user display name, domain and username are shown. Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|localSecurityOptionsLogOnMessageText|String|Set message text for users attempting to log in.|
|localSecurityOptionsLogOnMessageTitle|String|Set message title for users attempting to log in.|
|localSecurityOptionsMachineInactivityLimit|Int32|Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs. Valid values 0 to 9999|
|localSecurityOptionsMachineInactivityLimitInMinutes|Int32|Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs. Valid values 0 to 9999|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients|Enumeration|This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security. Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers|Enumeration|This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security. Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|localSecurityOptionsOnlyElevateSignedExecutables|Boolean|Enforce PKI certification path validation for a given executable file before it is permitted to run.|
|localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares|Boolean|By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously|
|localSecurityOptionsSmartCardRemovalBehavior|Enumeration|This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader. Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|localSecurityOptionsStandardUserElevationPromptBehavior|Enumeration|Define the behavior of the elevation prompt for standard users. Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation|Boolean|Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop. Prompt behavior policy settings for admins and standard users are used.|
|localSecurityOptionsUseAdminApprovalMode|Boolean|Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled|
|localSecurityOptionsUseAdminApprovalModeForAdministrators|Boolean|Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled|
|localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations|Boolean|Virtualize file and registry write failures to per user locations|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|smartScreenBlockOverrideForFiles|Boolean|Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.|
|smartScreenEnableInShell|Boolean|Allows IT Admins to configure SmartScreen for Windows.|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userRightsAccessCredentialManagerAsTrustedCaller|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right is used by Credential Manager during Backup/Restore. Users' saved credentials might be compromised if this privilege is given to other entities. Only states NotConfigured and Allowed are supported|
|userRightsActAsPartOfTheOperatingSystem|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right allows a process to impersonate any user without authentication. The process can therefore gain access to the same local resources as that user. Only states NotConfigured and Allowed are supported|
|userRightsAllowAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups are allowed to connect to the computer over the network. State Allowed is supported.|
|userRightsBackupData|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories. Only states NotConfigured and Allowed are supported|
|userRightsBlockAccessFromNetwork|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups are block from connecting to the computer over the network. State Block is supported.|
|userRightsChangeSystemTime|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups can change the time and date on the internal clock of the computer. Only states NotConfigured and Allowed are supported|
|userRightsCreateGlobalObjects|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This security setting determines whether users can create global objects that are available to all sessions. Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption. Only states NotConfigured and Allowed are supported|
|userRightsCreatePageFile|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups can call an internal API to create and change the size of a page file. Only states NotConfigured and Allowed are supported|
|userRightsCreatePermanentSharedObjects|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which accounts can be used by processes to create a directory object using the object manager. Only states NotConfigured and Allowed are supported|
|userRightsCreateSymbolicLinks|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines if the user can create a symbolic link from the computer to which they are logged on. Only states NotConfigured and Allowed are supported|
|userRightsCreateToken|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token. Only states NotConfigured and Allowed are supported|
|userRightsDebugPrograms|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can attach a debugger to any process or to the kernel. Only states NotConfigured and Allowed are supported|
|userRightsDelegation|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can set the Trusted for Delegation setting on a user or computer object. Only states NotConfigured and Allowed are supported.|
|userRightsDenyLocalLogOn|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users cannot log on to the computer. States NotConfigured, Blocked are supported |
|userRightsGenerateSecurityAudits|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which accounts can be used by a process to add entries to the security log. The security log is used to trace unauthorized system access.  Only states NotConfigured and Allowed are supported.|
|userRightsImpersonateClient|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|Assigning this user right to a user allows programs running on behalf of that user to impersonate a client. Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels. Only states NotConfigured and Allowed are supported.|
|userRightsIncreaseSchedulingPriority|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process. Only states NotConfigured and Allowed are supported.|
|userRightsLoadUnloadDrivers|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode. Only states NotConfigured and Allowed are supported.|
|userRightsLocalLogOn|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can log on to the computer. States NotConfigured, Allowed are supported |
|userRightsLockMemory|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk. Only states NotConfigured and Allowed are supported.|
|userRightsManageAuditingAndSecurityLogs|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys. Only states NotConfigured and Allowed are supported.|
|userRightsManageVolumes|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation. Only states NotConfigured and Allowed are supported.|
|userRightsModifyFirmwareEnvironment|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines who can modify firmware environment values. Only states NotConfigured and Allowed are supported.|
|userRightsModifyObjectLabels|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users. Only states NotConfigured and Allowed are supported.|
|userRightsProfileSingleProcess|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can use performance monitoring tools to monitor the performance of system processes. Only states NotConfigured and Allowed are supported.|
|userRightsRemoteDesktopServicesLogOn|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client. Only states NotConfigured and Blocked are supported|
|userRightsRemoteShutdown|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users are allowed to shut down a computer from a remote location on the network. Misuse of this user right can result in a denial of service. Only states NotConfigured and Allowed are supported.|
|userRightsRestoreData|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object. Only states NotConfigured and Allowed are supported.|
|userRightsTakeOwnership|[deviceManagementUserRightsSetting](../resources/deviceManagementUserRightsSetting.md)|This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads. Only states NotConfigured and Allowed are supported.|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|windowsDefenderTamperProtection|Enumeration|Configure windows defender TamperProtection settings. Possible values are: `notConfigured`, `enable`, `disable`.|
|xboxServicesAccessoryManagementServiceStartupMode|Enumeration|This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4). Default: Manual. Possible values are: `manual`, `automatic`, `disabled`.|
|xboxServicesEnableXboxGameSaveTask|Boolean|This setting determines whether xbox game save is enabled (1) or disabled (0).|
|xboxServicesLiveAuthManagerServiceStartupMode|Enumeration|This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4). Default: Manual. Possible values are: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveGameSaveServiceStartupMode|Enumeration|This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4). Default: Manual. Possible values are: `manual`, `automatic`, `disabled`.|
|xboxServicesLiveNetworkingServiceStartupMode|Enumeration|This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4). Default: Manual. Possible values are: `manual`, `automatic`, `disabled`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/deviceConfigurationAssignment.md) collection|The list of assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/settingStateDeviceSummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/deviceConfigurationDeviceStatus.md) collection|Device configuration installation status by device. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/deviceConfigurationDeviceOverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/deviceConfigurationGroupAssignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/deviceConfigurationUserStatus.md) collection|Device configuration installation status by user. Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/deviceConfigurationUserOverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/deviceConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration",
  "baseType": "microsoft.graph.deviceConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "edgeTraversal": "String",
      "localUserAuthorizations": "String"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "windowsDefenderTamperProtection": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
  },
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "String",
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "requireEncryptionForWriteAccess": true
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "String",
  "defenderDisableScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 1024,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderScanDirection": "String",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanDay": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderSubmitSamplesConsentType": "String",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  }
}
```

