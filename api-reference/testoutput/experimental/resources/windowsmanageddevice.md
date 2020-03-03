---
title: "windowsManagedDevice resource type"
description: "Windows devices that are managed or pre-enrolled through Intune"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsManagedDevice resource type


Namespace: microsoft.graph

Windows devices that are managed or pre-enrolled through Intune


Inherits from [managedDevice](../resources/manageddevice.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List windowsManagedDevices](../api/windowsmanageddevice-list.md)|[windowsManagedDevice](../resources/windowsmanageddevice.md) collection|List properties and relationships of the [windowsManagedDevice](../resources/windowsmanageddevice.md) objects.|
|[Get windowsManagedDevice](../api/windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/windowsmanageddevice.md)|Read properties and relationships of the [windowsManagedDevice](../resources/windowsmanageddevice.md) object.|
|[Create windowsManagedDevice](../api/windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/windowsmanageddevice.md)|Create a new [windowsManagedDevice](../resources/windowsmanageddevice.md) object.|
|[Delete windowsManagedDevice](../api/windowsmanageddevice-delete.md)|None|Deletes a [windowsManagedDevice](../resources/windowsmanageddevice.md).|
|[Update windowsManagedDevice](../api/windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/windowsmanageddevice.md)|Update the properties of a [windowsManagedDevice](../resources/windowsmanageddevice.md) object.|
|[overrideComplianceState](../api/windowsmanageddevice-overridecompliancestate.md)|None||
|[enableLostMode](../api/windowsmanageddevice-enablelostmode.md)|None||
|[playLostModeSound](../api/windowsmanageddevice-playlostmodesound.md)|None||
|[setDeviceName](../api/windowsmanageddevice-setdevicename.md)|None||
|[rotateFileVaultKey](../api/windowsmanageddevice-rotatefilevaultkey.md)|None||
|[getFileVaultKey](../api/windowsmanageddevice-getfilevaultkey.md)|String||
|[retire](../api/windowsmanageddevice-retire.md)|None||
|[wipe](../api/windowsmanageddevice-wipe.md)|None||
|[resetPasscode](../api/windowsmanageddevice-resetpasscode.md)|None||
|[remoteLock](../api/windowsmanageddevice-remotelock.md)|None||
|[requestRemoteAssistance](../api/windowsmanageddevice-requestremoteassistance.md)|None||
|[disableLostMode](../api/windowsmanageddevice-disablelostmode.md)|None||
|[locateDevice](../api/windowsmanageddevice-locatedevice.md)|None||
|[bypassActivationLock](../api/windowsmanageddevice-bypassactivationlock.md)|None||
|[rebootNow](../api/windowsmanageddevice-rebootnow.md)|None||
|[shutDown](../api/windowsmanageddevice-shutdown.md)|None||
|[recoverPasscode](../api/windowsmanageddevice-recoverpasscode.md)|None||
|[cleanWindowsDevice](../api/windowsmanageddevice-cleanwindowsdevice.md)|None||
|[logoutSharedAppleDeviceActiveUser](../api/windowsmanageddevice-logoutsharedappledeviceactiveuser.md)|None||
|[deleteUserFromSharedAppleDevice](../api/windowsmanageddevice-deleteuserfromsharedappledevice.md)|None||
|[syncDevice](../api/windowsmanageddevice-syncdevice.md)|None||
|[windowsDefenderScan](../api/windowsmanageddevice-windowsdefenderscan.md)|None||
|[windowsDefenderUpdateSignatures](../api/windowsmanageddevice-windowsdefenderupdatesignatures.md)|None||
|[updateWindowsDeviceAccount](../api/windowsmanageddevice-updatewindowsdeviceaccount.md)|None||
|[revokeAppleVppLicenses](../api/windowsmanageddevice-revokeapplevpplicenses.md)|None||
|[rotateBitLockerKeys](../api/windowsmanageddevice-rotatebitlockerkeys.md)|None||
|[sendCustomNotificationToCompanyPortal](../api/windowsmanageddevice-sendcustomnotificationtocompanyportal.md)|None||
|[triggerConfigurationManagerAction](../api/windowsmanageddevice-triggerconfigurationmanageraction.md)|None||
|[List securityBaselineStates](../api/windowsmanageddevice-list-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md) collection|Get the securityBaselineStates from the securityBaselineStates navigation property.|
|[Add securityBaselineStates](../api/windowsmanageddevice-post-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Add securityBaselineStates by posting to the securityBaselineStates collection.|
|[List deviceConfigurationStates](../api/windowsmanageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Add deviceConfigurationStates](../api/windowsmanageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Add deviceConfigurationStates by posting to the deviceConfigurationStates collection.|
|[List deviceCompliancePolicyStates](../api/windowsmanageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Add deviceCompliancePolicyStates](../api/windowsmanageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Add deviceCompliancePolicyStates by posting to the deviceCompliancePolicyStates collection.|
|[List managedDeviceMobileAppConfigurationStates](../api/windowsmanageddevice-list-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Get the managedDeviceMobileAppConfigurationStates from the managedDeviceMobileAppConfigurationStates navigation property.|
|[Add managedDeviceMobileAppConfigurationStates](../api/windowsmanageddevice-post-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Add managedDeviceMobileAppConfigurationStates by posting to the managedDeviceMobileAppConfigurationStates collection.|
|[List detectedApps](../api/windowsmanageddevice-list-detectedapps.md)|[detectedApp](../resources/intune-devices-detectedapp.md) collection|Get the detectedApps from the detectedApps navigation property.|
|[Create detectedApps](../api/windowsmanageddevice-post-detectedapps.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Create detectedApps by posting to the detectedApps collection.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read properties and relationships of the [deviceCategory](../resources/devicecategory.md) object.|
|[Get windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.|
|[List users](../api/windowsmanageddevice-list-users.md)|[user](../resources/user.md) collection|Get the users from the users navigation property.|
|[Add users](../api/windowsmanageddevice-post-users.md)|[user](../resources/user.md)|Add users by posting to the users collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aadRegistered|Boolean|Whether the device is Azure Active Directory registered. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|activationLockBypassCode|String|Code that allows the Activation Lock on a device to be bypassed. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Android security patch level. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolean|Reports if the managed device is enrolled via auto-pilot. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|The unique identifier for the Azure Active Directory device. Read only. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|The unique identifier for the Azure Active Directory device. Read only. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Whether the device is Azure Active Directory registered. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|Enumeration|Chassis type of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceState|Enumeration|Compliance state of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr client enabled features. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection|List of ComplexType deviceActionResult objects. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategoryDisplayName|String|Device category display name. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|Enumeration|Enrollment type of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|The device health attestation state. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Name of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|Enumeration|Device registration state. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceType|Enumeration|Platform of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|easActivated|Boolean|Whether the device is Exchange ActiveSync activated. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Exchange ActivationSync activation time of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|Exchange ActiveSync Id of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Email(s) for the user associated with the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|enrolledDateTime|DateTimeOffset|Enrollment time of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|ethernetMacAddress|String|Ethernet MAC. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|Enumeration|The Access State of the device in Exchange. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|Enumeration|The reason for the device's access state in Exchange. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Last time the device contacted Exchange. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Free Storage in Bytes. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|The hardward details for the device.  Includes information such as storage space, manufacturer, serial number, etc. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|String|Integrated Circuit Card Identifier, it is A SIM card's unique identification number. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|imei|String|IMEI. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Device encryption status. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Device supervised status. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|jailBroken|String|whether the device is jail broken or rooted. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|The date and time that the device last completed a successful sync with Intune. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|lostModeState|Enumeration|Indicates if Lost mode is enabled or disabled. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `disabled`, `enabled`.|
|managedDeviceName|String|Automatically generated name to identify a device. Can be overwritten to a user friendly name. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceOwnerType|Enumeration|Ownership of the device. Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `company`, `personal`.|
|managementAgent|Enumeration|Management channel of the device. Intune, EAS, etc. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|managementCertificateExpirationDate|DateTimeOffset|Reports device management certificate expiration date. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|Enumeration|Management state of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|manufacturer|String|Manufacturer of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|Model of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|operatingSystem|String|Operating system of the device. Windows, iOS, etc. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|osVersion|String|Operating system version of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|Enumeration|Ownership of the device. Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `company`, `personal`.|
|partnerReportedThreatState|Enumeration|Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read Only. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|phoneNumber|String|Phone number of the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|physicalMemoryInBytes|Int64|Total Memory in Bytes. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Reports the DateTime the preferMdmOverGroupPolicy setting was set.  When set, the Intune MDM settings will override Group Policy settings if there is a conflict. Read Only. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|processorArchitecture|Enumeration|Processor architecture. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md). Possible values are: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|remoteAssistanceSessionErrorDetails|String|An error string that identifies issues when creating Remote Assistance session objects. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionUrl|String|Url that allows a Remote Assistance session to be established with the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|Reports if the managed iOS device is user approval enrollment. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|retireAfterDateTime|DateTimeOffset|Indicates the time after when a device will be auto retired because of scheduled action. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this Device instance. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|String|SerialNumber. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Subscriber Carrier. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Total Storage in Bytes. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|udid|String|Unique Device Identifier for iOS and macOS devices. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|User display name. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Unique Identifier for the user associated with the device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Device user principal name. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection|Indicates the last logged on users of a device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Count of active malware for this windows device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Count of remediated malware for this windows device. This property is read-only. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) collection|All applications currently installed on the device Inherited from [managedDevice](../resources/manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/devicecategory.md)|Device category Inherited from [managedDevice](../resources/manageddevice.md)|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Device compliance policy states for this device. Inherited from [managedDevice](../resources/manageddevice.md)|
|deviceConfigurationStates|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Device configuration states for this device. Inherited from [managedDevice](../resources/manageddevice.md)|
|managedDeviceMobileAppConfigurationStates|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Managed device mobile app configuration states for this device. Inherited from [managedDevice](../resources/manageddevice.md)|
|securityBaselineStates|[securityBaselineState](../resources/securitybaselinestate.md) collection|Security baseline states for this device. Inherited from [managedDevice](../resources/manageddevice.md)|
|users|[user](../resources/user.md) collection|The primary users associated with the managed device. Inherited from [managedDevice](../resources/manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|The device protection status. Inherited from [managedDevice](../resources/manageddevice.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice",
  "baseType": "microsoft.graph.managedDevice",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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
    "clientIdentifier": "String"
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String"
}
```

