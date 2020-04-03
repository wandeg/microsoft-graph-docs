---
title: "Update deviceManagementSettingCategory"
description: "Update the properties of a deviceManagementSettingCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementSettingCategory

Namespace: microsoft.graph

Update the properties of a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.

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
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|hasRequiredSetting|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementsettingcategory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "1b6a14af-14af-1b6a-af14-6a1baf146a1b",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

