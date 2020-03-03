---
title: "Create resourceSpecificPermissionGrant"
description: "Create a new resourceSpecificPermissionGrant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create resourceSpecificPermissionGrant

Namespace: microsoft.graph

Create a new [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object.

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
POST /permissionGrants
POST /groups/{groupsId}/permissionGrants
POST /me/joinedGroups/{groupId}/permissionGrants
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_resourcespecificpermissiongrant_from_permissiongrants"
}
-->
``` http
POST https://graph.microsoft.com/localtest/permissionGrants
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.resourcespecificpermissiongrant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
  "id": "35c79838-9838-35c7-3898-c7353898c735",
  "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
  "clientId": "Client Id value",
  "clientAppId": "Client App Id value",
  "resourceAppId": "Resource App Id value",
  "permissionType": "Permission Type value",
  "permission": "Permission value"
}
```

