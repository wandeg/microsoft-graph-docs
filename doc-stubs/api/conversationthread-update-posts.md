---
title: "Update posts"
description: "Update the properties of a posts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update posts

Namespace: microsoft.graph

Update the properties of a posts object.

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
PATCH /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `200 OK` response code and an updated [post](../resources/post.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_posts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts
Content-Type: application/json
Content-length: 579

{
  "@odata.type": "#microsoft.graph.post",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

