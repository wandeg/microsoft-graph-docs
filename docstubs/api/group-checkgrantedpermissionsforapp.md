---
title: "group: checkGrantedPermissionsForApp"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_checkgrantedpermissionsforapp"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/checkGrantedPermissionsForApp
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.resourcespecificpermissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 448

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
      "id": "130cad0c-ad0c-130c-0cad-0c130cad0c13",
      "deletedDateTime": "2017-01-01T00:00:54.363956+03:00",
      "clientId": "Client Id value",
      "clientAppId": "Client App Id value",
      "resourceAppId": "Resource App Id value",
      "permissionType": "Permission Type value",
      "permission": "Permission value"
    }
  ]
}
```

