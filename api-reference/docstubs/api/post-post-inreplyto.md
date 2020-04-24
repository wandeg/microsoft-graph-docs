---
title: "Create inReplyTo"
description: "Create a new inReplyTo object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create inReplyTo

Namespace: microsoft.graph

Create a new inReplyTo object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [post](../resources/post.md) object.

The following table shows the properties that are required when you create the [post](../resources/post.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|receivedDateTime|DateTimeOffset|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|from|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|sender|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|conversationThreadId|String|**TODO: Add Description**|
|newParticipants|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|conversationId|String|**TODO: Add Description**|
|importance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|



## Response
If successful, this method returns a `201 Created` response code and a [post](../resources/post.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_post_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/inReplyTo
Content-Type: application/json
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
  "receivedDateTime": "2016-12-31T23:59:11.8329415+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.post",
  "id": "2f5989b0-89b0-2f59-b089-592fb089592f",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "receivedDateTime": "2016-12-31T23:59:11.8329415+03:00",
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

