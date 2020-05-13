---
title: "Update managedDevices"
description: "Update the properties of a managedDevices object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update managedDevices

Namespace: microsoft.graph

Update the properties of a managedDevices object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/managedDevices
PATCH /users/{usersId}/managedDevices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDevice](../resources/intune-manageddevice.md) object.

The following table shows the properties that are required when you create the [managedDevice](../resources/intune-manageddevice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|managedDeviceOwnerType|managedDeviceOwnerType|**TODO: Add Description**. Possible values are: `unknown`, `company`, `personal`.|
|deviceActionResults|[deviceActionResult](../resources/intune-deviceactionresult.md) collection|**TODO: Add Description**|
|enrolledDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|operatingSystem|String|**TODO: Add Description**|
|complianceState|complianceState|**TODO: Add Description**. Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|**TODO: Add Description**|
|managementAgent|managementAgentType|**TODO: Add Description**. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|osVersion|String|**TODO: Add Description**|
|easActivated|Boolean|**TODO: Add Description**|
|easDeviceId|String|**TODO: Add Description**|
|easActivationDateTime|DateTimeOffset|**TODO: Add Description**|
|azureADRegistered|Boolean|**TODO: Add Description**|
|deviceEnrollmentType|deviceEnrollmentType|**TODO: Add Description**. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|activationLockBypassCode|String|**TODO: Add Description**|
|emailAddress|String|**TODO: Add Description**|
|azureADDeviceId|String|**TODO: Add Description**|
|deviceRegistrationState|deviceRegistrationState|**TODO: Add Description**. Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|**TODO: Add Description**|
|isSupervised|Boolean|**TODO: Add Description**|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|exchangeAccessState|deviceManagementExchangeAccessState|**TODO: Add Description**. Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|deviceManagementExchangeAccessStateReason|**TODO: Add Description**. Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|**TODO: Add Description**|
|remoteAssistanceSessionErrorDetails|String|**TODO: Add Description**|
|isEncrypted|Boolean|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|imei|String|**TODO: Add Description**|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|androidSecurityPatchLevel|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-configurationmanagerclientenabledfeatures.md)|**TODO: Add Description**|
|wiFiMacAddress|String|**TODO: Add Description**|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devicehealthattestationstate.md)|**TODO: Add Description**|
|subscriberCarrier|String|**TODO: Add Description**|
|meid|String|**TODO: Add Description**|
|totalStorageSpaceInBytes|Int64|**TODO: Add Description**|
|freeStorageSpaceInBytes|Int64|**TODO: Add Description**|
|managedDeviceName|String|**TODO: Add Description**|
|partnerReportedThreatState|managedDevicePartnerReportedHealthState|**TODO: Add Description**. Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-manageddevice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_manageddevices"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/managedDevices
Content-Type: application/json
Content-length: 1946

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": "Boolean",
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": "Boolean",
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
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
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": "Integer",
  "freeStorageSpaceInBytes": "Integer",
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "45c55459-5459-45c5-5954-c5455954c545",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": "Boolean",
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": "Boolean",
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
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
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": "Integer",
  "freeStorageSpaceInBytes": "Integer",
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```

