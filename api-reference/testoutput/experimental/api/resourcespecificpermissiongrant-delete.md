---
title: "Delete resourceSpecificPermissionGrant"
description: "Deletes a resourceSpecificPermissionGrant."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete resourceSpecificPermissionGrant

Namespace: microsoft.graph

Deletes a [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md).

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
DELETE /permissionGrants/{permissionGrantsId}
DELETE /groups/{groupsId}/permissionGrants/{resourceSpecificPermissionGrantId}
DELETE /me/joinedGroups/{groupId}/permissionGrants/{resourceSpecificPermissionGrantId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_resourcespecificpermissiongrant"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/permissionGrants/{permissionGrantsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

