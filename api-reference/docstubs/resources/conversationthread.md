---
title: "conversationThread resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# conversationThread resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get conversationThread](../api/conversationthread-get.md)|[conversationThread](../resources/conversationthread.md)|Read properties and relationships of a [conversationThread](../resources/conversationthread.md) object.|
|[Update conversationThread](../api/conversationthread-update.md)|[conversationThread](../resources/conversationthread.md)|Update the properties of a [conversationThread](../resources/conversationthread.md) object.|
|[reply](../api/conversationthread-reply.md)|None|**TODO: Add Description**|
|[List posts](../api/conversationthread-list-posts.md)|[post](../resources/post.md) collection|Get the posts from the posts navigation property.|
|[Create posts](../api/conversationthread-post-posts.md)|[post](../resources/post.md)|Create a new posts object.|
|[Delete posts](../api/conversationthread-delete-posts.md)|None|Delete a posts object.|
|[Update posts](../api/conversationthread-update-posts.md)|[post](../resources/post.md)|Update the properties of a posts object.|
|[Get post](../api/post-get.md)|[post](../resources/post.md)|Read properties and relationships of a [post](../resources/post.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isLocked|Boolean|**TODO: Add Description**|
|lastDeliveredDateTime|DateTimeOffset|**TODO: Add Description**|
|preview|String|**TODO: Add Description**|
|topic|String|**TODO: Add Description**|
|toRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|uniqueSenders|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|posts|[post](../resources/post.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationThread",
  "id": "String (identifier)",
  "toRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "topic": "String",
  "hasAttachments": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "uniqueSenders": [
    "String"
  ],
  "ccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "preview": "String",
  "isLocked": true
}
```

