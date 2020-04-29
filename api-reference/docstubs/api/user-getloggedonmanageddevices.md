---
title: "user: getLoggedOnManagedDevices"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getLoggedOnManagedDevices

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/getLoggedOnManagedDevices
GET /users/{usersId}/getLoggedOnManagedDevices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/manageddevice.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_getloggedonmanageddevices"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getLoggedOnManagedDevices
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "String (identifier)",
      "userId": "String",
      "deviceName": "String",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation"
      },
      "ownerType": "String",
      "managedDeviceOwnerType": "String",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult"
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
      "partnerReportedThreatState": "String",
      "retireAfterDateTime": "String (timestamp)",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser"
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
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation"
      },
      "ethernetMacAddress": "String",
      "physicalMemoryInBytes": "Integer",
      "processorArchitecture": "String",
      "specificationVersion": "String"
    }
  ]
}
```

