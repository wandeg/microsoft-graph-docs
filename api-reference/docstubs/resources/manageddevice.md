---
title: "managedDevice resource type"
description: "Devices that are managed or pre-enrolled through Intune"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# managedDevice resource type


Namespace: microsoft.graph

Devices that are managed or pre-enrolled through Intune


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read properties and relationships of a [managedDevice](../resources/manageddevice.md) object.|
|[Update managedDevice](../api/manageddevice-update.md)|[managedDevice](../resources/manageddevice.md)|Update the properties of a [managedDevice](../resources/manageddevice.md) object.|
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
|[List deviceConfigurationStates](../api/manageddevice-list-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Get the deviceConfigurationStates from the deviceConfigurationStates navigation property.|
|[Create deviceConfigurationStates](../api/manageddevice-post-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Create a new deviceConfigurationStates object.|
|[Delete deviceConfigurationStates](../api/manageddevice-delete-deviceconfigurationstates.md)|None|Delete a deviceConfigurationStates object.|
|[Update deviceConfigurationStates](../api/manageddevice-update-deviceconfigurationstates.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Update the properties of a deviceConfigurationStates object.|
|[Get deviceConfigurationState](../api/deviceconfigurationstate-get.md)|[deviceConfigurationState](../resources/deviceconfigurationstate.md)|Read properties and relationships of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Create deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Create a new deviceCompliancePolicyStates object.|
|[Delete deviceCompliancePolicyStates](../api/manageddevice-delete-devicecompliancepolicystates.md)|None|Delete a deviceCompliancePolicyStates object.|
|[Update deviceCompliancePolicyStates](../api/manageddevice-update-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Update the properties of a deviceCompliancePolicyStates object.|
|[Get deviceCompliancePolicyState](../api/devicecompliancepolicystate-get.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Read properties and relationships of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[List deviceCategory](../api/manageddevice-list-devicecategory.md)|[deviceCategory](../resources/devicecategory.md) collection|Get the deviceCategories from the deviceCategory navigation property.|
|[Create deviceCategory](../api/manageddevice-post-devicecategory.md)|[deviceCategory](../resources/devicecategory.md)|Create a new deviceCategory object.|
|[Delete deviceCategory](../api/manageddevice-delete-devicecategory.md)|None|Delete a deviceCategory object.|
|[Update deviceCategory](../api/manageddevice-update-devicecategory.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a deviceCategory object.|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read properties and relationships of a [deviceCategory](../resources/devicecategory.md) object.|
|[List managedDevices](../api/user-list-manageddevices.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevices navigation property.|
|[Create managedDevices](../api/user-post-manageddevices.md)|[managedDevice](../resources/manageddevice.md)|Create a new managedDevices object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activationLockBypassCode|String|Code that allows the Activation Lock on a device to be bypassed.|
|androidSecurityPatchLevel|String|Android security patch level|
|azureADDeviceId|String|The unique identifier for the Azure Active Directory device. Read only.|
|azureADRegistered|Boolean|Whether the device is Azure Active Directory registered.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|complianceState|complianceState|Compliance state of the device. Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/configurationmanagerclientenabledfeatures.md)|ConfigrMgr client enabled features|
|deviceActionResults|[deviceActionResult](../resources/deviceactionresult.md) collection|List of ComplexType deviceActionResult objects.|
|deviceCategoryDisplayName|String|Device category display name|
|deviceEnrollmentType|deviceEnrollmentType|Enrollment type of the device. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/devicehealthattestationstate.md)|The device health attestation state.|
|deviceName|String|Name of the device|
|deviceRegistrationState|deviceRegistrationState|Device registration state. Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|easActivated|Boolean|Whether the device is Exchange ActiveSync activated.|
|easActivationDateTime|DateTimeOffset|Exchange ActivationSync activation time of the device.|
|easDeviceId|String|Exchange ActiveSync Id of the device.|
|emailAddress|String|Email(s) for the user associated with the device|
|enrolledDateTime|DateTimeOffset|Enrollment time of the device.|
|exchangeAccessState|deviceManagementExchangeAccessState|The Access State of the device in Exchange. Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|deviceManagementExchangeAccessStateReason|The reason for the device's access state in Exchange. Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Last time the device contacted Exchange.|
|freeStorageSpaceInBytes|Int64|Free Storage in Bytes|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|imei|String|IMEI|
|isEncrypted|Boolean|Device encryption status|
|isSupervised|Boolean|Device supervised status|
|jailBroken|String|whether the device is jail broken or rooted.|
|lastSyncDateTime|DateTimeOffset|The date and time that the device last completed a successful sync with Intune.|
|managedDeviceName|String|Automatically generated name to identify a device. Can be overwritten to a user friendly name.|
|managedDeviceOwnerType|managedDeviceOwnerType|Ownership of the device. Can be 'company' or 'personal'. Possible values are: `unknown`, `company`, `personal`.|
|managementAgent|managementAgentType|Management channel of the device. Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|manufacturer|String|Manufacturer of the device|
|meid|String|MEID|
|model|String|Model of the device|
|operatingSystem|String|Operating system of the device. Windows, iOS, etc.|
|osVersion|String|Operating system version of the device.|
|partnerReportedThreatState|managedDevicePartnerReportedHealthState|Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read Only. Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|phoneNumber|String|Phone number of the device|
|remoteAssistanceSessionErrorDetails|String|An error string that identifies issues when creating Remote Assistance session objects.|
|remoteAssistanceSessionUrl|String|Url that allows a Remote Assistance session to be established with the device.|
|serialNumber|String|SerialNumber|
|subscriberCarrier|String|Subscriber Carrier|
|totalStorageSpaceInBytes|Int64|Total Storage in Bytes|
|userDisplayName|String|User display name|
|userId|String|Unique Identifier for the user associated with the device|
|userPrincipalName|String|Device user principal name|
|wiFiMacAddress|String|Wi-Fi MAC|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/devicecategory.md)|Device category|
|deviceCompliancePolicyStates|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Device compliance policy states for this device.|
|deviceConfigurationStates|[deviceConfigurationState](../resources/deviceconfigurationstate.md) collection|Device configuration states for this device.|

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
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
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
    "windowsUpdateForBusiness": true
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
  "partnerReportedThreatState": "String"
}
```

