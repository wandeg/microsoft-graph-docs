---
title: "Get deviceConfigurationState"
description: "Read the properties and relationships of a deviceConfigurationState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceConfigurationState

Namespace: microsoft.graph

Read the properties and relationships of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.

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
GET /me/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
GET /users/{usersId}/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
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

If successful, this method returns a `200 OK` response code and a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_deviceconfigurationstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationState",
    "id": "f63435ac-35ac-f634-ac35-34f6ac3534f6",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
      }
    ],
    "displayName": "String",
    "version": "Integer",
    "platformType": "String",
    "state": "String",
    "settingCount": "Integer",
    "userId": "String",
    "userPrincipalName": "String"
  }
}
```

