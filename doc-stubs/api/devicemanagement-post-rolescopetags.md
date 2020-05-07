---
title: "Create roleScopeTags"
description: "Create a new roleScopeTags object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create roleScopeTags

Namespace: microsoft.graph

Create a new roleScopeTags object.

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
POST /deviceManagement/roleScopeTags
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [roleScopeTag](../resources/rolescopetag.md) object.

The following table shows the properties that are required when you create the [roleScopeTag](../resources/rolescopetag.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|isBuiltIn|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/rolescopetag.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_rolescopetag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rolescopetag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "aa3b0004-0004-aa3b-0400-3baa04003baa",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": "Boolean"
}
```

