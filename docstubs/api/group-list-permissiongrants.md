---
title: "List permissionGrants"
description: "Get the resourceSpecificPermissionGrants from the permissionGrants navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List permissionGrants

Namespace: microsoft.graph

Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.

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
GET /groups/{groupsId}/permissionGrants
GET /me/joinedGroups/{groupId}/permissionGrants
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_resourcespecificpermissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/permissionGrants
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
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
      "id": "819e7522-7522-819e-2275-9e8122759e81",
      "deletedDateTime": "2016-12-31T23:58:28.3197258+03:00",
      "clientId": "Client Id value",
      "clientAppId": "Client App Id value",
      "resourceAppId": "Resource App Id value",
      "permissionType": "Permission Type value",
      "permission": "Permission value"
    }
  ]
}
```

