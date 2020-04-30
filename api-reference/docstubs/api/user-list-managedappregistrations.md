---
title: "List managedAppRegistrations"
description: "Get the managedAppRegistrations from the managedAppRegistrations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List managedAppRegistrations

Namespace: microsoft.graph

Get the managedAppRegistrations from the managedAppRegistrations navigation property.

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
GET /me/managedAppRegistrations
GET /users/{usersId}/managedAppRegistrations
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
If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/managedappregistration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managedappregistration"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedAppRegistrations
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedappregistration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
      "id": "f21a0c3f-0c3f-f21a-3f0c-1af23f0c1af2",
      "createdDateTime": "String (timestamp)",
      "lastSyncDateTime": "String (timestamp)",
      "applicationVersion": "String",
      "managementSdkVersion": "String",
      "platformVersion": "String",
      "deviceType": "String",
      "deviceTag": "String",
      "deviceName": "String",
      "managedDeviceId": "String",
      "azureADDeviceId": "String",
      "deviceModel": "String",
      "deviceManufacturer": "String",
      "flaggedReasons": [
        "String"
      ],
      "userId": "String",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "version": "String"
    }
  ]
}
```

