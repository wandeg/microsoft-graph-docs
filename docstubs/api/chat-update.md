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
|Name|Description|
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
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/{chatsId}
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "c45e2dd5-2dd5-c45e-d52d-5ec4d52d5ec4",
  "topic": "Topic value",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00"
}
```

