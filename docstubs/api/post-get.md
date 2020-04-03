---
title: "Get post"
description: "Read properties and relationships of the post object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get post

Namespace: microsoft.graph

Read properties and relationships of the [post](../resources/post.md) object.

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
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
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
If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_post"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1116

{
  "value": {
    "@odata.type": "#microsoft.graph.post",
    "id": "01eb9832-9832-01eb-3298-eb013298eb01",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "receivedDateTime": "2017-01-01T00:01:26.5638837+00:00",
    "hasAttachments": true,
    "from": {
      "@odata.type": "microsoft.graph.recipient",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      }
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

