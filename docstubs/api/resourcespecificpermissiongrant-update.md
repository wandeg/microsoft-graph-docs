---
title: "Update resourceSpecificPermissionGrant"
description: "Update the properties of a resourceSpecificPermissionGrant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update resourceSpecificPermissionGrant

Namespace: microsoft.graph

Update the properties of a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

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
PATCH /permissionGrants/{permissionGrantsId}
PATCH /groups/{groupsId}/permissionGrants/{resourceSpecificPermissionGrantId}
PATCH /me/joinedGroups/{groupId}/permissionGrants/{resourceSpecificPermissionGrantId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

The following table shows the properties that are required when you create the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|clientId|String||
|clientAppId|String||
|resourceAppId|String||
|permissionType|String||
|permission|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_resourcespecificpermissiongrant"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/permissionGrants/{permissionGrantsId}
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
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
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "c2ce095b-095b-c2ce-5b09-cec25b09cec2",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

