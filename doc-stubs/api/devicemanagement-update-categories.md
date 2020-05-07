---
title: "Update categories"
description: "Update the properties of a categories object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update categories

Namespace: microsoft.graph

Update the properties of a categories object.

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
PATCH /deviceManagement/categories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.

The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|hasRequiredSetting|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_categories"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "String",
  "hasRequiredSetting": "Boolean"
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
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "3f7a89b2-89b2-3f7a-b289-7a3fb2897a3f",
  "displayName": "String",
  "hasRequiredSetting": "Boolean"
}
```

