---
title: "List channels"
description: "Get the channels from the channels navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List channels

Namespace: microsoft.graph

Get the channels from the channels navigation property.

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
GET /teams/{teamsId}/channels
GET /me/joinedGroups/{groupId}/team/channels
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [channel](../resources/channel.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_channel"
}
-->
``` http
GET https://graph.microsoft.com/localtest/teams/{teamsId}/channels
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.channel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.channel",
      "id": "c6b8902d-902d-c6b8-2d90-b8c62d90b8c6",
      "displayName": "Display Name value",
      "description": "Description value",
      "isFavoriteByDefault": true,
      "email": "Email value",
      "webUrl": "https://example.com/webUrl/",
      "membershipType": "String"
    }
  ]
}
```

