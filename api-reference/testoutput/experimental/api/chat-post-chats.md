---
title: "Create chat"
description: "Create a new chat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create chat

Namespace: microsoft.graph

Create a new [chat](../resources/chat.md) object.

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
POST /chats
POST /me/chats
POST /users/{usersId}/chats
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [chat](../resources/chat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_chat_from_chats"
}
-->
``` http
POST https://graph.microsoft.com/localtest/chats
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00"
}
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.chat",
  "id": "819136cf-36cf-8191-cf36-9181cf369181",
  "topic": "Topic value",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00"
}
```

