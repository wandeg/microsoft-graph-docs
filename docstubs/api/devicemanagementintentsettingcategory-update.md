---
title: "Update deviceManagementIntentSettingCategory"
description: "Update the properties of a deviceManagementIntentSettingCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementIntentSettingCategory

Namespace: microsoft.graph

Update the properties of a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|hasRequiredSetting|Boolean| Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementintentsettingcategory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}
Content-type: application/json
Content-length: 150

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 199

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "a1f78ccb-8ccb-a1f7-cb8c-f7a1cb8cf7a1",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

