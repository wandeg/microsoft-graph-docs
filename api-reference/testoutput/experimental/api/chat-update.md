---
title: "Update chat"
description: "Update the properties of a chat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update chat

Namespace: microsoft.graph

Update the properties of a [chat](../resources/chat.md) object.

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
PATCH /chats/{chatsId}
PATCH /me/chats/{chatId}
PATCH /users/{usersId}/chats/{chatId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [chat](../resources/chat.md) object.

The following table shows the properties that are required when you create the [chat](../resources/chat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|topic|String||
|createdDateTime|DateTimeOffset||
|lastUpdatedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [chat](../resources/chat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/chats/{chatsId}
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2017-01-01T00:02:06.1258154+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "@odata.type": "#microsoft.graph.chat",
  "id": "28220fd3-0fd3-2822-d30f-2228d30f2228",
  "topic": "Topic value",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastUpdatedDateTime": "2017-01-01T00:02:06.1258154+03:00"
}
```

