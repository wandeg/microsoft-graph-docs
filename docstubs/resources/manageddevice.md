---
title: "managedDevice resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDevice resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read properties and relationships of the [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevice](../api/manageddevice-update.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a [managedDevice](../resources/manageddevice.md) object.|
|[overrideComplianceState](../api/manageddevice-overridecompliancestate.md)|None||
|[enableLostMode](../api/manageddevice-enablelostmode.md)|None||
|[playLostModeSound](../api/manageddevice-playlostmodesound.md)|None||
|[setDeviceName](../api/manageddevice-setdevicename.md)|None||
|[rotateFileVaultKey](../api/manageddevice-rotatefilevaultkey.md)|None||
|[getFileVaultKey](../api/manageddevice-getfilevaultkey.md)|String||
|[retire](../api/manageddevice-retire.md)|None||
|[wipe](../api/manageddevice-wipe.md)|None||
|[resetPasscode](../api/manageddevice-resetpasscode.md)|None||
|[remoteLock](../api/manageddevice-remotelock.md)|None||
|[requestRemoteAssistance](../api/manageddevice-requestremoteassistance.md)|None||
|[disableLostMode](../api/manageddevice-disablelostmode.md)|None||
|[locateDevice](../api/manageddevice-locatedevice.md)|None||
|[bypassActivationLock](../api/manageddevice-bypassactivationlock.md)|None||
|[rebootNow](../api/manageddevice-rebootnow.md)|None||
|[shutDown](../api/manageddevice-shutdown.md)|None||
|[recoverPasscode](../api/manageddevice-recoverpasscode.md)|None||
|[cleanWindowsDevice](../api/manageddevice-cleanwindowsdevice.md)|None||
|[logoutSharedAppleDeviceActiveUser](../api/manageddevice-logoutsharedappledeviceactiveuser.md)|None||
|[deleteUserFromSharedAppleDevice](../api/manageddevice-deleteuserfromsharedappledevice.md)|None||
|[syncDevice](../api/manageddevice-syncdevice.md)|None||
|[windowsDefenderScan](../api/manageddevice-windowsdefenderscan.md)|None||
|[windowsDefenderUpdateSignatures](../api/manageddevice-windowsdefenderupdatesignatures.md)|None||
|[updateWindowsDeviceAccount](../api/manageddevice-updatewindowsdeviceaccount.md)|None||
|[revokeAppleVppLicenses](../api/manageddevice-revokeapplevpplicenses.md)|None||
|[rotateBitLockerKeys](../api/manageddevice-rotatebitlockerkeys.md)|None||
|[sendCustomNotificationToCompanyPortal](../api/manageddevice-sendcustomnotificationtocompanyportal.md)|None||
|[triggerConfigurationManagerAction](../api/manageddevice-triggerconfigurationmanageraction.md)|None||
|[executeAction](../api/manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/bulkmanageddeviceactionresult.md)||
|[List securityBaselineStates](../api/manageddevice-list-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md) collection|Get the securityBaselineStates from the securityBaselineStates navigation property.|
|[Add securityBaselineStates](../api/manageddevice-post-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Add securityBaselineStates by posting to the securityBaselineStates collection.|
|[List deviceConfigurationStates](../api/manageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Add deviceConfigurationStates](../api/manageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Add deviceConfigurationStates by posting to the deviceConfigurationStates collection.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Add deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Add deviceCompliancePolicyStates by posting to the deviceCompliancePolicyStates collection.|
|[List managedDeviceMobileAppConfigurationStates](../api/manageddevice-list-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Get the managedDeviceMobileAppConfigurationStates from the managedDeviceMobileAppConfigurationStates navigation property.|
|[Add managedDeviceMobileAppConfigurationStates](../api/manageddevice-post-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Add managedDeviceMobileAppConfigurationStates by posting to the managedDeviceMobileAppConfigurationStates collection.|
|[List detectedApps](../api/manageddevice-list-detectedapps.md)|[detectedApp](../resources/detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Create detectedApps](../api/manageddevice-post-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Create detectedApps by posting to the detectedApps collection.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read properties and relationships of the [deviceCategory](../resources/devicecategory.md) object.|
|[Get windowsProtectionState](../api/windowsprotectionstate-get.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Read properties and relationships of the [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[List users](../api/manageddevice-list-users.md)|[user](../resources/user.md) collection|Get the users from the users navigation property.|
|[Add users](../api/manageddevice-post-users.md)|[user](../resources/user.md)|Add users by posting to the users collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aadRegistered|Boolean||
|activationLockBypassCode|String||
|androidSecurityPatchLevel|String||
|autopilotEnrolled|Boolean||
|azureActiveDirectoryDeviceId|String||
|azureADDeviceId|String||
|azureADRegistered|Boolean||
|chassisType|Enumeration| Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset||
|complianceState|Enumeration| Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/configurationmanagerclientenabledfeatures.md)||
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/configurationmanagerclienthealthstate.md)||
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/configurationmanagerclientinformation.md)||
|deviceActionResults|[deviceActionResult](../resources/deviceactionresult.md) collection||
|deviceCategoryDisplayName|String||
|deviceEnrollmentType|Enumeration| Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/devicehealthattestationstate.md)||
|deviceName|String||
|deviceRegistrationState|Enumeration| Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceType|Enumeration| Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.|
|easActivated|Boolean||
|easActivationDateTime|DateTimeOffset||
|easDeviceId|String||
|emailAddress|String||
|enrolledDateTime|DateTimeOffset||
|ethernetMacAddress|String||
|exchangeAccessState|Enumeration| Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|Enumeration| Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset||
|freeStorageSpaceInBytes|Int64||
|hardwareInformation|[hardwareInformation](../resources/hardwareinformation.md)||
|iccid|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|imei|String||
|isEncrypted|Boolean||
|isSupervised|Boolean||
|jailBroken|String||
|lastSyncDateTime|DateTimeOffset||
|lostModeState|Enumeration| Possible values are: `disabled`, `enabled`.|
|managedDeviceName|String||
|managedDeviceOwnerType|Enumeration| Possible values are: `unknown`, `company`, `personal`.|
|managementAgent|Enumeration| Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|managementCertificateExpirationDate|DateTimeOffset||
|managementState|Enumeration| Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|manufacturer|String||
|meid|String||
|model|String||
|notes|String||
|operatingSystem|String||
|osVersion|String||
|ownerType|Enumeration| Possible values are: `unknown`, `company`, `personal`.|
|partnerReportedThreatState|Enumeration| Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|phoneNumber|String||
|physicalMemoryInBytes|Int64||
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset||
|processorArchitecture|Enumeration| Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|remoteAssistanceSessionErrorDetails|String||
|remoteAssistanceSessionUrl|String||
|requireUserEnrollmentApproval|Boolean||
|retireAfterDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|serialNumber|String||
|subscriberCarrier|String||
|totalStorageSpaceInBytes|Int64||
|udid|String||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||
|usersLoggedOn|[loggedOnUser](../resources/loggedonuser.md) collection||
|wiFiMacAddress|String||
|windowsActiveMalwareCount|Int32||
|windowsRemediatedMalwareCount|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/detectedapp.md) collection||
|deviceCategory|[deviceCategory](../resources/devicecategory.md)||
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection||
|deviceConfigurationStates|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection||
|managedDeviceMobileAppConfigurationStates|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection||
|securityBaselineStates|[securityBaselineState](../resources/securitybaselinestate.md) collection||
|users|[user](../resources/user.md) collection||
|windowsProtectionState|[windowsProtectionState](../resources/windowsprotectionstate.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String",
    "isBlocked": true
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String"
}
```

