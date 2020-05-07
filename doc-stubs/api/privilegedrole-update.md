---
title: "Update privilegedRole"
description: "Update the properties of a privilegedRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedRole

Namespace: microsoft.graph

Update the properties of a [privilegedRole](../resources/privilegedrole.md) object.

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
PATCH /privilegedRoles/{privilegedRolesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [privilegedRole](../resources/privilegedrole.md) object.

The following table shows the properties that are required when you create the [privilegedRole](../resources/privilegedrole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [privilegedRole](../resources/privilegedrole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedrole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}
Content-Type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "name": "String"
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
  "@odata.type": "#microsoft.graph.privilegedRole",
  "id": "123d2107-2107-123d-0721-3d1207213d12",
  "name": "String"
}
```

