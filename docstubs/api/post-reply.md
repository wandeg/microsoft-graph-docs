---
title: "reply"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# reply

Namespace: microsoft.graph



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
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/reply
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo/reply
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|Post|[post](../resources/post.md)||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "post_reply"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/reply

Content-type: application/json
Content-length: 889

{
  "Post": {
    "@odata.type": "#microsoft.graph.post",
    "id": "a651c8aa-c8aa-a651-aac8-51a6aac851a6",
    "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "receivedDateTime": "2017-01-01T00:00:39.8035424+03:00",
    "hasAttachments": true,
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "conversationThreadId": "Conversation Thread Id value",
    "newParticipants": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "Conversation Id value",
    "importance": "String"
  }
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
HTTP/1.1 204 No Content
```

