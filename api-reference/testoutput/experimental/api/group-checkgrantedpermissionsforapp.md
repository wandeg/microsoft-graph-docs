---
title: "checkGrantedPermissionsForApp"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# checkGrantedPermissionsForApp

Namespace: microsoft.graph



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
POST /groups/{groupsId}/checkGrantedPermissionsForApp
POST /me/joinedGroups/{groupId}/checkGrantedPermissionsForApp
POST /users/{usersId}/joinedGroups/{groupId}/checkGrantedPermissionsForApp
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "group_checkgrantedpermissionsforapp"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groups/{groupsId}/checkGrantedPermissionsForApp
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.resourcespecificpermissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 449

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
      "id": "87f4d19e-d19e-87f4-9ed1-f4879ed1f487",
      "deletedDateTime": "2016-12-31T23:57:45.8652256+03:00",
      "clientId": "Client Id value",
      "clientAppId": "Client App Id value",
      "resourceAppId": "Resource App Id value",
      "permissionType": "Permission Type value",
      "permission": "Permission value"
    }
  ]
}
```

