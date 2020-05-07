---
title: "Create managedDeviceMobileAppConfigurationStates"
description: "Create a new managedDeviceMobileAppConfigurationStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedDeviceMobileAppConfigurationStates

Namespace: microsoft.graph

Create a new managedDeviceMobileAppConfigurationStates object.

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
POST /users/{usersId}/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.

The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingStates|[managedDeviceMobileAppConfigurationSettingState](../resources/manageddevicemobileappconfigurationsettingstate.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|state|complianceStatus|**TODO: Add Description**. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddevicemobileappconfigurationstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
Content-Type: application/json
Content-length: 403

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
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
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddevicemobileappconfigurationstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "88ed80a9-80a9-88ed-a980-ed88a980ed88",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
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

