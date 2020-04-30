---
title: "Update permissionGrants"
description: "Update the properties of a permissionGrants object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update permissionGrants

Namespace: microsoft.graph

Update the properties of a permissionGrants object.

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
PATCH ** Collection URI for microsoft.graph.resourceSpecificPermissionGrant not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

The following table shows the properties that are required when you create the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|clientId|String|**TODO: Add Description**|
|clientAppId|String|**TODO: Add Description**|
|resourceAppId|String|**TODO: Add Description**|
|permissionType|String|**TODO: Add Description**|
|permission|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_permissiongrants"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.resourceSpecificPermissionGrant not found
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
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
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "c5a0e21c-e21c-c5a0-1ce2-a0c51ce2a0c5",
  "deletedDateTime": "String (timestamp)",
  "clientId": "String",
  "clientAppId": "String",
  "resourceAppId": "String",
  "permissionType": "String",
  "permission": "String"
}
```

