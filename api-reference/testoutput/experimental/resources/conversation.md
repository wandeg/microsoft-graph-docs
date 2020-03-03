---
title: "conversation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# conversation resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get conversation](../api/conversation-get.md)|[conversation](../resources/conversation.md)|Read properties and relationships of the [conversation](../resources/conversation.md) object.|
|[Delete conversation](../api/conversation-delete.md)|None|Deletes a [conversation](../resources/conversation.md).|
|[Update conversation](../api/conversation-update.md)|[conversation](../resources/conversation.md)|Update the properties of a [conversation](../resources/conversation.md) object.|
|[List threads](../api/conversation-list-threads.md)|[conversationThread](../resources/conversationThread.md) collection|Get the conversationThreads from the threads navigation property.|
|[Add threads](../api/conversation-post-threads.md)|[conversationThread](../resources/conversationThread.md)|Add threads by posting to the threads collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hasAttachments|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastDeliveredDateTime|DateTimeOffset||
|preview|String||
|topic|String||
|uniqueSenders|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|threads|[conversationThread](../resources/conversationThread.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversation",
  "id": "String (identifier)",
  "topic": "String",
  "hasAttachments": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "uniqueSenders": [
    "String"
  ],
  "preview": "String"
}
```

