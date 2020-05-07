---
title: "managedDevice resource type"
description: "Devices that are managed or pre-enrolled through Intune"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDevice resource type


Namespace: microsoft.graph

Devices that are managed or pre-enrolled through Intune

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[executeAction](../api/manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/bulkmanageddeviceactionresult.md)|**TODO: Add Description**|
|[enableLostMode](../api/manageddevice-enablelostmode.md)|None|Enable lost mode|
|[playLostModeSound](../api/manageddevice-playlostmodesound.md)|None|Remote lock|
|[setDeviceName](../api/manageddevice-setdevicename.md)|None|Set device name of the device.|
|[rotateFileVaultKey](../api/manageddevice-rotatefilevaultkey.md)|None|**TODO: Add Description**|
|[getFileVaultKey](../api/manageddevice-getfilevaultkey.md)|String|**TODO: Add Description**|
|[retire](../api/manageddevice-retire.md)|None|Retire a device|
|[wipe](../api/manageddevice-wipe.md)|None|Wipe a device|
|[resetPasscode](../api/manageddevice-resetpasscode.md)|None|Reset passcode|
|[remoteLock](../api/manageddevice-remotelock.md)|None|Remote lock|
|[requestRemoteAssistance](../api/manageddevice-requestremoteassistance.md)|None|Request remote assistance|
|[disableLostMode](../api/manageddevice-disablelostmode.md)|None|Disable lost mode|
|[locateDevice](../api/manageddevice-locatedevice.md)|None|Locate a device|
|[bypassActivationLock](../api/manageddevice-bypassactivationlock.md)|None|Bypass activation lock|
|[rebootNow](../api/manageddevice-rebootnow.md)|None|Reboot device|
|[shutDown](../api/manageddevice-shutdown.md)|None|Shut down device|
|[recoverPasscode](../api/manageddevice-recoverpasscode.md)|None|Recover passcode|
|[cleanWindowsDevice](../api/manageddevice-cleanwindowsdevice.md)|None|Clean Windows device|
|[logoutSharedAppleDeviceActiveUser](../api/manageddevice-logoutsharedappledeviceactiveuser.md)|None|Logout shared Apple device active user|
|[deleteUserFromSharedAppleDevice](../api/manageddevice-deleteuserfromsharedappledevice.md)|None|Delete user from shared Apple device|
|[syncDevice](../api/manageddevice-syncdevice.md)|None|**TODO: Add Description**|
|[windowsDefenderScan](../api/manageddevice-windowsdefenderscan.md)|None|**TODO: Add Description**|
|[windowsDefenderUpdateSignatures](../api/manageddevice-windowsdefenderupdatesignatures.md)|None|**TODO: Add Description**|
|[updateWindowsDeviceAccount](../api/manageddevice-updatewindowsdeviceaccount.md)|None|**TODO: Add Description**|
|[revokeAppleVppLicenses](../api/manageddevice-revokeapplevpplicenses.md)|None|Revoke all Apple Vpp licenses for a device|
|[rotateBitLockerKeys](../api/manageddevice-rotatebitlockerkeys.md)|None|Rotate BitLockerKeys|
|[sendCustomNotificationToCompanyPortal](../api/manageddevice-sendcustomnotificationtocompanyportal.md)|None|**TODO: Add Description**|
|[triggerConfigurationManagerAction](../api/manageddevice-triggerconfigurationmanageraction.md)|None|Trigger action on ConfigurationManager client|
|[List detectedApps](../api/manageddevice-list-detectedapps.md)|[detectedApp](../resources/detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Add detectedApps](../api/manageddevice-post-detectedapps.md)|[detectedApp](../resources/detectedapp.md)|Add detectedApps by posting to the detectedApps collection.|
|[Remove detectedApps](../api/manageddevice-delete-detectedapps.md)|None|Remove a [detectedApp](../resources/detectedapp.md) object.|
|[List deviceCategory](../api/manageddevice-list-devicecategory.md)|[deviceCategory](../resources/devicecategory.md) collection|Get the deviceCategories from the deviceCategory navigation property.|
|[Create deviceCategory](../api/manageddevice-post-devicecategory.md)|[deviceCategory](../resources/devicecategory.md)|Create a new deviceCategory object.|
|[Delete deviceCategory](../api/manageddevice-delete-devicecategory.md)|None|Delete a [deviceCategory](../resources/devicecategory.md) object.|
|[Update deviceCategory](../api/manageddevice-update-devicecategory.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a deviceCategory object.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read the properties and relationships of a [deviceCategory](../resources/devicecategory.md) object.|
|[List windowsProtectionState](../api/manageddevice-list-windowsprotectionstate.md)|[windowsProtectionState](../resources/windowsprotectionstate.md) collection|Get the windowsProtectionStates from the windowsProtectionState navigation property.|
|[Create windowsProtectionState](../api/manageddevice-post-windowsprotectionstate.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Create a new windowsProtectionState object.|
|[Delete windowsProtectionState](../api/manageddevice-delete-windowsprotectionstate.md)|None|Delete a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[Update windowsProtectionState](../api/manageddevice-update-windowsprotectionstate.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Update the properties of a windowsProtectionState object.|
|[Get windowsProtectionState](../api/windowsprotectionstate-get.md)|[windowsProtectionState](../resources/windowsprotectionstate.md)|Read the properties and relationships of a [windowsProtectionState](../resources/windowsprotectionstate.md) object.|
|[List users](../api/manageddevice-list-users.md)|[user](../resources/user.md) collection|Get the users from the users navigation property.|
|[Create users](../api/manageddevice-post-users.md)|[user](../resources/user.md)|Create a new users object.|
|[Delete users](../api/manageddevice-delete-users.md)|None|Delete a [user](../resources/user.md) object.|
|[Update users](../api/manageddevice-update-users.md)|[user](../resources/user.md)|Update the properties of a users object.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read the properties and relationships of a [user](../resources/user.md) object.|
|[List managedDevices](../api/detectedapp-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Add managedDevices](../api/detectedapp-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Add managedDevices by posting to the managedDevices collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aadRegistered|Boolean|Whether the device is Azure Active Directory registered. This property is read-only.|
|activationLockBypassCode|String|Code that allows the Activation Lock on a device to be bypassed. This property is read-only.|
|androidSecurityPatchLevel|String|Android security patch level. This property is read-only.|
|autopilotEnrolled|Boolean|Reports if the managed device is enrolled via auto-pilot. This property is read-only.|
|azureActiveDirectoryDeviceId|String|The unique identifier for the Azure Active Directory device. Read only. This property is read-only.|
|azureADDeviceId|String|The unique identifier for the Azure Active Directory device. Read only. This property is read-only.|
|azureADRegistered|Boolean|Whether the device is Azure Active Directory registered. This property is read-only.|
|chassisType|chassisType|Chassis type of the device. This property is read-only. Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires. This property is read-only.|
|complianceState|complianceState|Compliance state of the device. This property is read-only. Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/configurationmanagerclientenabledfeatures.md)|ConfigrMgr client enabled features. This property is read-only.|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/configurationmanagerclienthealthstate.md)|Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/configurationmanagerclientinformation.md)|Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent|
|deviceActionResults|[deviceActionResult](../resources/deviceactionresult.md) collection|List of ComplexType deviceActionResult objects. This property is read-only.|
|deviceCategoryDisplayName|String|Device category display name. This property is read-only.|
|deviceEnrollmentType|deviceEnrollmentType|Enrollment type of the device. This property is read-only. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/devicehealthattestationstate.md)|The device health attestation state. This property is read-only.|
|deviceName|String|Name of the device. This property is read-only.|
|deviceRegistrationState|deviceRegistrationState|Device registration state. This property is read-only. Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceType|deviceType|Platform of the device. This property is read-only. Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.|
|easActivated|Boolean|Whether the device is Exchange ActiveSync activated. This property is read-only.|
|easActivationDateTime|DateTimeOffset|Exchange ActivationSync activation time of the device. This property is read-only.|
|easDeviceId|String|Exchange ActiveSync Id of the device. This property is read-only.|
|emailAddress|String|Email(s) for the user associated with the device. This property is read-only.|
|enrolledDateTime|DateTimeOffset|Enrollment time of the device. This property is read-only.|
|ethernetMacAddress|String|Ethernet MAC. This property is read-only.|
|exchangeAccessState|deviceManagementExchangeAccessState|The Access State of the device in Exchange. This property is read-only. Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|deviceManagementExchangeAccessStateReason|The reason for the device's access state in Exchange. This property is read-only. Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Last time the device contacted Exchange. This property is read-only.|
|freeStorageSpaceInBytes|Int64|Free Storage in Bytes. This property is read-only.|
|hardwareInformation|[hardwareInformation](../resources/hardwareinformation.md)|The hardward details for the device.  Includes information such as storage space, manufacturer, serial number, etc. This property is read-only.|
|iccid|String|Integrated Circuit Card Identifier, it is A SIM card's unique identification number. This property is read-only.|
|id|String|Unique Identifier for the device. This property is read-only.|
|imei|String|IMEI. This property is read-only.|
|isEncrypted|Boolean|Device encryption status. This property is read-only.|
|isSupervised|Boolean|Device supervised status. This property is read-only.|
|jailBroken|String|whether the device is jail broken or rooted. This property is read-only.|
|lastSyncDateTime|DateTimeOffset|The date and time that the device last completed a successful sync with Intune. This property is read-only.|
|lostModeState|lostModeState|Indicates if Lost mode is enabled or disabled. This property is read-only. Possible values are: `disabled`, `enabled`.|
|managedDeviceName|String|Automatically generated name to identify a device. Can be overwritten to a user friendly name.|
|managedDeviceOwnerType|managedDeviceOwnerType|Ownership of the device. Can be 'company' or 'personal'. Possible values are: `unknown`, `company`, `personal`.|
|managementAgent|managementAgentType|Management channel of the device. Intune, EAS, etc. This property is read-only. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.|
|managementCertificateExpirationDate|DateTimeOffset|Reports device management certificate expiration date. This property is read-only.|
|managementState|managementState|Management state of the device. This property is read-only. Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|manufacturer|String|Manufacturer of the device. This property is read-only.|
|meid|String|MEID. This property is read-only.|
|model|String|Model of the device. This property is read-only.|
|notes|String|Notes on the device created by IT Admin|
|operatingSystem|String|Operating system of the device. Windows, iOS, etc. This property is read-only.|
|osVersion|String|Operating system version of the device. This property is read-only.|
|ownerType|ownerType|Ownership of the device. Can be 'company' or 'personal'. Possible values are: `unknown`, `company`, `personal`.|
|partnerReportedThreatState|managedDevicePartnerReportedHealthState|Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read Only. This property is read-only. Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|phoneNumber|String|Phone number of the device. This property is read-only.|
|physicalMemoryInBytes|Int64|Total Memory in Bytes. This property is read-only.|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Reports the DateTime the preferMdmOverGroupPolicy setting was set.  When set, the Intune MDM settings will override Group Policy settings if there is a conflict. Read Only. This property is read-only.|
|processorArchitecture|managedDeviceArchitecture|Processor architecture. This property is read-only. Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|remoteAssistanceSessionErrorDetails|String|An error string that identifies issues when creating Remote Assistance session objects. This property is read-only.|
|remoteAssistanceSessionUrl|String|Url that allows a Remote Assistance session to be established with the device. This property is read-only.|
|requireUserEnrollmentApproval|Boolean|Reports if the managed iOS device is user approval enrollment. This property is read-only.|
|retireAfterDateTime|DateTimeOffset|Indicates the time after when a device will be auto retired because of scheduled action. This property is read-only.|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this Device instance.|
|serialNumber|String|SerialNumber. This property is read-only.|
|specificationVersion|String|Specification version. This property is read-only.|
|subscriberCarrier|String|Subscriber Carrier. This property is read-only.|
|totalStorageSpaceInBytes|Int64|Total Storage in Bytes. This property is read-only.|
|udid|String|Unique Device Identifier for iOS and macOS devices. This property is read-only.|
|userDisplayName|String|User display name. This property is read-only.|
|userId|String|Unique Identifier for the user associated with the device. This property is read-only.|
|userPrincipalName|String|Device user principal name. This property is read-only.|
|usersLoggedOn|[loggedOnUser](../resources/loggedonuser.md) collection|Indicates the last logged on users of a device. This property is read-only.|
|wiFiMacAddress|String|Wi-Fi MAC. This property is read-only.|
|windowsActiveMalwareCount|Int32|Count of active malware for this windows device. This property is read-only.|
|windowsRemediatedMalwareCount|Int32|Count of remediated malware for this windows device. This property is read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/detectedapp.md) collection|All applications currently installed on the device|
|deviceCategory|[deviceCategory](../resources/devicecategory.md)|Device category|
|users|[user](../resources/user.md) collection|The primary users associated with the managed device.|
|windowsProtectionState|[windowsProtectionState](../resources/windowsprotectionstate.md)|The device protection status.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.managedDevice",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.management.services.api.hardwareInformation"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.management.services.api.deviceActionResult"
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
  "easActivated": "Boolean",
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": "Boolean",
  "azureADRegistered": "Boolean",
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": "Boolean",
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": "Boolean",
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
    "@odata.type": "microsoft.management.services.api.configurationManagerClientEnabledFeatures"
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.management.services.api.deviceHealthAttestationState"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": "Integer",
  "freeStorageSpaceInBytes": "Integer",
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.management.services.api.loggedOnUser"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": "Boolean",
  "requireUserEnrollmentApproval": "Boolean",
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": "Integer",
  "windowsRemediatedMalwareCount": "Integer",
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.management.services.api.configurationManagerClientHealthState"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.management.services.api.configurationManagerClientInformation"
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": "Integer",
  "processorArchitecture": "String",
  "specificationVersion": "String"
}
```

