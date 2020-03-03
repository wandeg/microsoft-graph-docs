---
title: "Create deviceManagementSettingCategory"
description: "Create a new deviceManagementSettingCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceManagementSettingCategory

Namespace: microsoft.graph

Create a new [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/categories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The category name|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementsettingcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/categories
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementsettingcategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "fcc4bc02-bc02-fcc4-02bc-c4fc02bcc4fc",
  "displayName": "Display Name value"
}
```

