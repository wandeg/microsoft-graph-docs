---
title: "Add posts"
description: "Add posts by posting to the posts collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add posts

Add posts by posting to the posts collection.

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
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the post object.

The following table shows the properties that are required when you create the post.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookItem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookItem.md)|
|body|[itemBody](../resources/itemBody.md)||
|receivedDateTime|DateTimeOffset||
|hasAttachments|Boolean||
|from|[recipient](../resources/recipient.md)||
|sender|[recipient](../resources/recipient.md)||
|conversationThreadId|String||
|newParticipants|[recipient](../resources/recipient.md) collection||
|conversationId|String||
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|



## Response
If successful, this method returns a `201 Created` response code and a [post](../resources/post.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_post_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts
Content-type: application/json
Content-length: 857

{
  "@odata.type": "#microsoft.graph.post",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "receivedDateTime": "2016-12-31T23:59:48.3455349+03:00",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1029

{
  "@odata.type": "#microsoft.graph.post",
  "id": "1ee906f1-06f1-1ee9-f106-e91ef106e91e",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "receivedDateTime": "2016-12-31T23:59:48.3455349+03:00",
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
```

