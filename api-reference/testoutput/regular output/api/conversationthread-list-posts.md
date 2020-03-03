---
title: "List posts"
description: "Get the posts from the posts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List posts

Namespace: microsoft.graph

Get the posts from the posts navigation property.

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
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [post](../resources/post.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_post"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.post)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1166

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.post",
      "id": "9e5cddfc-ddfc-9e5c-fcdd-5c9efcdd5c9e",
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
      "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "body": {
        "@odata.type": "microsoft.graph.itemBody",
        "contentType": "String",
        "content": "Content value"
      },
      "receivedDateTime": "2017-01-01T00:01:55.9317761+03:00",
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
      "conversationId": "Conversation Id value"
    }
  ]
}
```

