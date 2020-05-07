---
title: "Update deviceConfigurationStates"
description: "Update the properties of a deviceConfigurationStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceConfigurationStates

Namespace: microsoft.graph

Update the properties of a deviceConfigurationStates object.

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
PATCH /users/{usersId}/managedDevices/{managedDeviceId}/deviceConfigurationStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationState](../resources/deviceconfigurationstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingStates|[deviceConfigurationSettingState](../resources/deviceconfigurationsettingstate.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|state|complianceStatus|**TODO: Add Description**. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationState](../resources/deviceconfigurationstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationstates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/deviceConfigurationStates
Content-Type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
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
```

