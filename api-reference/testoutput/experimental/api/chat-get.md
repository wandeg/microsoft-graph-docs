---
title: "Get chat"
description: "Read properties and relationships of the chat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get chat

Namespace: microsoft.graph

Read properties and relationships of the [chat](../resources/chat.md) object.

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
GET /chats/{chatsId}
GET /me/chats/{chatId}
GET /users/{usersId}/chats/{chatId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [chat](../resources/chat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/localtest/chats/{chatsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.chat",
    "id": "28220fd3-0fd3-2822-d30f-2228d30f2228",
    "topic": "Topic value",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastUpdatedDateTime": "2017-01-01T00:02:06.1258154+03:00"
  }
}
```

