---
title: "List windows10EndpointProtectionConfigurations"
description: "List properties and relationships of the windows10EndpointProtectionConfiguration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windows10EndpointProtectionConfigurations

Namespace: microsoft.graph

List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.windows10EndpointProtectionConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/windows10endpointprotectionconfiguration.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windows10endpointprotectionconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.windows10EndpointProtectionConfiguration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windows10endpointprotectionconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 20531

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
      "id": "8a306c39-6c39-8a30-396c-308a396c308a",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "String"
        ],
        "name": "Name value",
        "ruleType": "String"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "String"
      },
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "dmaGuardDeviceEnumerationPolicy": "String",
      "firewallRules": [
        {
          "@odata.type": "microsoft.graph.windowsFirewallRule",
          "packageFamilyName": "Package Family Name value",
          "filePath": "File Path value",
          "serviceName": "Service Name value",
          "protocol": 8,
          "localPortRanges": [
            "Local Port Ranges value"
          ],
          "remotePortRanges": [
            "Remote Port Ranges value"
          ],
          "localAddressRanges": [
            "Local Address Ranges value"
          ],
          "remoteAddressRanges": [
            "Remote Address Ranges value"
          ],
          "profileTypes": "String",
          "action": "String",
          "trafficDirection": "String",
          "interfaceTypes": "String",
          "edgeTraversal": "String",
          "localUserAuthorizations": "Local User Authorizations value"
        }
      ],
      "userRightsAccessCredentialManagerAsTrustedCaller": {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
        "state": "String",
        "localUsersOrGroups": [
          {
            "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
            "securityIdentifier": "Security Identifier value"
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
      "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
      "localSecurityOptionsDisableGuestAccount": true,
      "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
      "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
      "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
      "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
      "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
      "localSecurityOptionsMachineInactivityLimit": 10,
      "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
      "localSecurityOptionsDoNotRequireCtrlAltDel": true,
      "localSecurityOptionsHideLastSignedInUser": true,
      "localSecurityOptionsHideUsernameAtSignIn": true,
      "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
      "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
      "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
      "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
      "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
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
      "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
      "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
      "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
      "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
      "defenderSecurityCenterNotificationsFromApp": "String",
      "defenderSecurityCenterITContactDisplay": "String",
      "windowsDefenderTamperProtection": "String",
      "firewallBlockStatefulFTP": true,
      "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
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
        "Defender Attack Surface Reduction Excluded Paths value"
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
        "Defender Guarded Folders Allowed App Paths value"
      ],
      "defenderAdditionalGuardedFolders": [
        "Defender Additional Guarded Folders value"
      ],
      "defenderNetworkProtectionType": "String",
      "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
      "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
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
        "minimumPinLength": 0,
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
        "prebootRecoveryMessage": "Preboot Recovery Message value",
        "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
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
      "defenderScanMaxCpuPercentage": 12,
      "defenderCheckForSignaturesBeforeRunningScan": true,
      "defenderCloudBlockLevel": "String",
      "defenderCloudExtendedTimeoutInSeconds": 5,
      "defenderDaysBeforeDeletingQuarantinedMalware": 12,
      "defenderDisableCatchupFullScan": true,
      "defenderDisableCatchupQuickScan": true,
      "defenderEnableLowCpuPriority": true,
      "defenderFileExtensionsToExclude": [
        "Defender File Extensions To Exclude value"
      ],
      "defenderFilesAndFoldersToExclude": [
        "Defender Files And Folders To Exclude value"
      ],
      "defenderProcessesToExclude": [
        "Defender Processes To Exclude value"
      ],
      "defenderPotentiallyUnwantedAppAction": "String",
      "defenderScanDirection": "String",
      "defenderScanType": "String",
      "defenderScheduledQuickScanTime": "12:02:45.2150000",
      "defenderScheduledScanDay": "String",
      "defenderScheduledScanTime": "12:01:04.6330000",
      "defenderSubmitSamplesConsentType": "String",
      "defenderDetectedMalwareActions": {
        "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
        "lowSeverity": "String",
        "moderateSeverity": "String",
        "highSeverity": "String",
        "severeSeverity": "String"
      }
    }
  ]
}
```

