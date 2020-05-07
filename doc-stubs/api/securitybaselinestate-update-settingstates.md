---
title: "Update settingStates"
description: "Update the properties of a settingStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update settingStates

Namespace: microsoft.graph

Update the properties of a settingStates object.

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
PATCH /users/{usersId}/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.

The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/securitybaselinesettingstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingName|String|**TODO: Add Description**|
|state|securityBaselineComplianceState|**TODO: Add Description**. Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|settingCategoryId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_settingstates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
Content-Type: application/json
Content-length: 154

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
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
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "7e3078ec-78ec-7e30-ec78-307eec78307e",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```

