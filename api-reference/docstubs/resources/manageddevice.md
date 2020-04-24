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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read the properties and relationships of a [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevice](../api/manageddevice-update.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a [managedDevice](../resources/manageddevice.md) object.|
|[overrideComplianceState](../api/manageddevice-overridecompliancestate.md)|None|**TODO: Add Description**|
|[enableLostMode](../api/manageddevice-enablelostmode.md)|None|**TODO: Add Description**|
|[playLostModeSound](../api/manageddevice-playlostmodesound.md)|None|**TODO: Add Description**|
|[setDeviceName](../api/manageddevice-setdevicename.md)|None|**TODO: Add Description**|
|[rotateFileVaultKey](../api/manageddevice-rotatefilevaultkey.md)|None|**TODO: Add Description**|
|[getFileVaultKey](../api/manageddevice-getfilevaultkey.md)|String|**TODO: Add Description**|
|[retire](../api/manageddevice-retire.md)|None|**TODO: Add Description**|
|[wipe](../api/manageddevice-wipe.md)|None|**TODO: Add Description**|
|[resetPasscode](../api/manageddevice-resetpasscode.md)|None|**TODO: Add Description**|
|[remoteLock](../api/manageddevice-remotelock.md)|None|**TODO: Add Description**|
|[requestRemoteAssistance](../api/manageddevice-requestremoteassistance.md)|None|**TODO: Add Description**|
|[disableLostMode](../api/manageddevice-disablelostmode.md)|None|**TODO: Add Description**|
|[locateDevice](../api/manageddevice-locatedevice.md)|None|**TODO: Add Description**|
|[bypassActivationLock](../api/manageddevice-bypassactivationlock.md)|None|**TODO: Add Description**|
|[rebootNow](../api/manageddevice-rebootnow.md)|None|**TODO: Add Description**|
|[shutDown](../api/manageddevice-shutdown.md)|None|**TODO: Add Description**|
|[recoverPasscode](../api/manageddevice-recoverpasscode.md)|None|**TODO: Add Description**|
|[cleanWindowsDevice](../api/manageddevice-cleanwindowsdevice.md)|None|**TODO: Add Description**|
|[logoutSharedAppleDeviceActiveUser](../api/manageddevice-logoutsharedappledeviceactiveuser.md)|None|**TODO: Add Description**|
|[deleteUserFromSharedAppleDevice](../api/manageddevice-deleteuserfromsharedappledevice.md)|None|**TODO: Add Description**|
|[syncDevice](../api/manageddevice-syncdevice.md)|None|**TODO: Add Description**|
|[windowsDefenderScan](../api/manageddevice-windowsdefenderscan.md)|None|**TODO: Add Description**|
|[windowsDefenderUpdateSignatures](../api/manageddevice-windowsdefenderupdatesignatures.md)|None|**TODO: Add Description**|
|[updateWindowsDeviceAccount](../api/manageddevice-updatewindowsdeviceaccount.md)|None|**TODO: Add Description**|
|[revokeAppleVppLicenses](../api/manageddevice-revokeapplevpplicenses.md)|None|**TODO: Add Description**|
|[rotateBitLockerKeys](../api/manageddevice-rotatebitlockerkeys.md)|None|**TODO: Add Description**|
|[sendCustomNotificationToCompanyPortal](../api/manageddevice-sendcustomnotificationtocompanyportal.md)|None|**TODO: Add Description**|
|[triggerConfigurationManagerAction](../api/manageddevice-triggerconfigurationmanageraction.md)|None|**TODO: Add Description**|
|[executeAction](../api/manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/bulkmanageddeviceactionresult.md)|**TODO: Add Description**|
|[List securityBaselineStates](../api/manageddevice-list-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md) collection|Get the securityBaselineStates from the securityBaselineStates navigation property.|
|[Create securityBaselineStates](../api/manageddevice-post-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Create a new securityBaselineStates object.|
|[Delete securityBaselineStates](../api/manageddevice-delete-securitybaselinestates.md)|None|Delete a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[Update securityBaselineStates](../api/manageddevice-update-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Update the properties of a securityBaselineStates object.|
|[Get securityBaselineState](../api/securitybaselinestate-get.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Read the properties and relationships of a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[List deviceConfigurationStates](../api/manageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Create deviceConfigurationStates](../api/manageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Create a new deviceConfigurationStates object.|
|[Delete deviceConfigurationStates](../api/manageddevice-delete-deviceconfigurationstates.md)|None|Delete a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[Update deviceConfigurationStates](../api/manageddevice-update-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Update the properties of a deviceConfigurationStates object.|
|[Get deviceConfigurationState](../api/deviceconfigurationstate-get.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Read the properties and relationships of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Create deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Create a new deviceCompliancePolicyStates object.|
|[Delete deviceCompliancePolicyStates](../api/manageddevice-delete-devicecompliancepolicystates.md)|None|Delete a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[Update deviceCompliancePolicyStates](../api/manageddevice-update-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Update the properties of a deviceCompliancePolicyStates object.|
|[Get deviceCompliancePolicyState](../api/devicecompliancepolicystate-get.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Read the properties and relationships of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[List managedDeviceMobileAppConfigurationStates](../api/manageddevice-list-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Get the managedDeviceMobileAppConfigurationStates from the managedDeviceMobileAppConfigurationStates navigation property.|
|[Create managedDeviceMobileAppConfigurationStates](../api/manageddevice-post-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Create a new managedDeviceMobileAppConfigurationStates object.|
|[Delete managedDeviceMobileAppConfigurationStates](../api/manageddevice-delete-manageddevicemobileappconfigurationstates.md)|None|Delete a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|
|[Update managedDeviceMobileAppConfigurationStates](../api/manageddevice-update-manageddevicemobileappconfigurationstates.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Update the properties of a managedDeviceMobileAppConfigurationStates object.|
|[Get managedDeviceMobileAppConfigurationState](../api/manageddevicemobileappconfigurationstate-get.md)|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md)|Read the properties and relationships of a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.|
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
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Device compliance policy states for this device.|
|deviceConfigurationStates|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Device configuration states for this device.|
|managedDeviceMobileAppConfigurationStates|[managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) collection|Managed device mobile app configuration states for this device.|
|securityBaselineStates|[securityBaselineState](../resources/securitybaselinestate.md) collection|Security baseline states for this device.|
|users|[user](../resources/user.md) collection|The primary users associated with the managed device.|
|windowsProtectionState|[windowsProtectionState](../resources/windowsprotectionstate.md)|The device protection status.|

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
  "processorArchitecture": "String",
  "specificationVersion": "String"
}
```

