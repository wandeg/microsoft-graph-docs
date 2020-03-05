---
title: "List posts"
description: "List properties and relationships of the post objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List posts

Namespace: microsoft.graph

List properties and relationships of the [post](../resources/post.md) objects.

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

## Examples

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
Content-Length: 1165

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.post",
      "id": "54407219-7219-5440-1972-405419724054",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "body": {
        "@odata.type": "microsoft.graph.itemBody",
        "contentType": "String",
        "content": "Content value"
      },
      "receivedDateTime": "2017-01-01T00:02:50.2294959+03:00",
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

