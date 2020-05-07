---
title: "Get securityBaselineSettingState"
description: "Read the properties and relationships of a securityBaselineSettingState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get securityBaselineSettingState

Namespace: microsoft.graph

Read the properties and relationships of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.

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
GET /me/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
GET /users/{usersId}/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
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

If successful, this method returns a `200 OK` response code and a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_securitybaselinesettingstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineSettingState",
    "id": "7e3078ec-78ec-7e30-ec78-307eec78307e",
    "settingName": "String",
    "state": "String",
    "settingCategoryId": "String"
  }
}
```

