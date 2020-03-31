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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /chats
GET /me/chats
GET /users/{usersId}/chats
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
If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats
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
Content-Length: 297

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chat",
      "id": "c8b4c4a8-c4a8-c8b4-a8c4-b4c8a8c4b4c8",
      "topic": "Topic value",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "lastUpdatedDateTime": "2017-01-01T00:01:44.5765244+03:00"
    }
  ]
}
```

