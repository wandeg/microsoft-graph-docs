---
title: "List resourceSpecificPermissionGrants"
description: "List properties and relationships of the resourceSpecificPermissionGrant objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List resourceSpecificPermissionGrants

Namespace: microsoft.graph

List properties and relationships of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects.

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
GET /permissionGrants
GET /groups/{groupsId}/permissionGrants
GET /me/joinedGroups/{groupId}/permissionGrants
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_resourcespecificpermissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/beta/permissionGrants
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
      "id": "4b45c63a-c63a-4b45-3ac6-454b3ac6454b",
      "deletedDateTime": "2016-12-31T23:59:31.2455853+03:00",
      "clientId": "Client Id value",
      "clientAppId": "Client App Id value",
      "resourceAppId": "Resource App Id value",
      "permissionType": "Permission Type value",
      "permission": "Permission value"
    }
  ]
}
```

