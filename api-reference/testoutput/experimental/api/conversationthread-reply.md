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
POST /groups/{groupsId}/threads/{conversationThreadId}/reply
POST /me/joinedGroups/{groupId}/threads/{conversationThreadId}/reply
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/reply
```

## Request headers
|Header|Value|
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
  "name": "conversationthread_reply"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groups/{groupsId}/threads/{conversationThreadId}/reply

Content-type: application/json
Content-length: 957

{
  "Post": {
    "@odata.type": "#microsoft.graph.post",
    "id": "f2546f32-6f32-f254-326f-54f2326f54f2",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "receivedDateTime": "2016-12-31T23:59:18.1123015+03:00",
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

