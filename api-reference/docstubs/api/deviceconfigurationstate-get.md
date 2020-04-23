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
GET /invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
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
    "id": "13b634b5-34b5-13b6-b534-b613b534b613",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
        "setting": "Setting value",
        "settingName": "Setting Name value",
        "instanceDisplayName": "Instance Display Name value",
        "state": "String",
        "errorCode": 9,
        "errorDescription": "Error Description value",
        "userId": "User Id value",
        "userName": "User Name value",
        "userEmail": "User Email value",
        "userPrincipalName": "User Principal Name value",
        "sources": [
          {
            "@odata.type": "microsoft.graph.settingSource",
            "id": "Id value",
            "displayName": "Display Name value"
          }
        ],
        "currentValue": "Current Value value"
      }
    ],
    "displayName": "Display Name value",
    "version": 7,
    "platformType": "String",
    "state": "String",
    "settingCount": 12
  }
}
```

