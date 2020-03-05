---
title: "List profilePhotos"
description: "List properties and relationships of the profilePhoto objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List profilePhotos

Namespace: microsoft.graph

List properties and relationships of the [profilePhoto](../resources/profilephoto.md) objects.

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
GET /me/photos
GET /users/{usersId}/photos
GET /groups/{groupsId}/photos
GET /me/joinedTeams/{groupId}/photos
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_profilephoto"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/photos
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.profilephoto)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 183

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.profilePhoto",
      "id": "a24ba7a6-a7a6-a24b-a6a7-4ba2a6a74ba2",
      "height": 6,
      "width": 5
    }
  ]
}
```

