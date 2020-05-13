---
title: "List managedDevices"
description: "Get the managedDevices from the managedDevices navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedDevices

Namespace: microsoft.graph

Get the managedDevices from the managedDevices navigation property.

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
GET /me/managedDevices
GET /users/{usersId}/managedDevices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/manageddevice.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_manageddevice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/managedDevices
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
      "id": "5af982b3-82b3-5af9-b382-f95ab382f95a",
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
  ]
}
```

