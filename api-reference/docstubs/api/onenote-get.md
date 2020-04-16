---
title: "Get onenote"
description: "Read properties and relationships of an onenote object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenote

Namespace: microsoft.graph

Read properties and relationships of an [onenote](../resources/onenote.md) object.

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
GET /me/onenote
GET /users/{usersId}/onenote
GET /sites/{sitesId}/onenote
GET /groups/{groupsId}/onenote
GET /me/joinedGroups/{groupId}/onenote
GET /me/joinedGroups/{groupId}/sites/{siteId}/onenote
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
If successful, this method returns a `200 OK` response code and an [onenote](../resources/onenote.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onenote"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/onenote
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenote"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.onenote",
    "id": "b2ec96a8-96a8-b2ec-a896-ecb2a896ecb2"
  }
}
```

