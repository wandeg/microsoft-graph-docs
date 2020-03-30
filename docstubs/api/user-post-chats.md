---
title: "Add chats"
description: "Add chats by posting to the chats collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add chats

Namespace: microsoft.graph

Add chats by posting to the chats collection.

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
POST /me/chats/$ref
POST /users/{usersId}/chats/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_chat_from_chats"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/chats
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2017-01-01T00:01:50.447451+00:00"
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
  "id": "f0e32e2f-2e2f-f0e3-2f2e-e3f02f2ee3f0",
  "topic": "Topic value",
  "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
  "lastUpdatedDateTime": "2017-01-01T00:01:50.447451+00:00"
}
```

