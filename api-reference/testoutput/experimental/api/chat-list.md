---
title: "List chats"
description: "List properties and relationships of the chat objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List chats

Namespace: microsoft.graph

List properties and relationships of the [chat](../resources/chat.md) objects.

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
GET /chats
GET /me/chats
GET /users/{usersId}/chats
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/localtest/chats
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 296

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chat",
      "id": "819136cf-36cf-8191-cf36-9181cf369181",
      "topic": "Topic value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00"
    }
  ]
}
```

