---
title: "Get post"
description: "Read the properties and relationships of a post object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get post

Namespace: microsoft.graph

Read the properties and relationships of a [post](../resources/post.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [post](../resources/post.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_post"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.post",
    "id": "4b0f40da-40da-4b0f-da40-0f4bda400f4b",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "changeKey": "String",
    "categories": [
      "String"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "receivedDateTime": "String (timestamp)",
    "hasAttachments": "Boolean",
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "conversationThreadId": "String",
    "newParticipants": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "String",
    "importance": "String"
  }
}
```

