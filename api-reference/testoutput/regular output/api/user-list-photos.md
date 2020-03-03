---
title: "List photos"
description: "Get the profilePhotos from the photos navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List photos

Namespace: microsoft.graph

Get the profilePhotos from the photos navigation property.

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
GET /me/photos
GET /users/{usersId}/photos
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.

## Example

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
      "id": "ee96df92-df92-ee96-92df-96ee92df96ee",
      "height": 6,
      "width": 5
    }
  ]
}
```

