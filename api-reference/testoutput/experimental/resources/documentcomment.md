---
title: "documentComment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# documentComment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get documentComment](../api/documentcomment-get.md)|[documentComment](../resources/documentComment.md)|Read properties and relationships of the [documentComment](../resources/documentcomment.md) object.|
|[Delete documentComment](../api/documentcomment-delete.md)|None|Deletes a [documentComment](../resources/documentcomment.md).|
|[Update documentComment](../api/documentcomment-update.md)|[documentComment](../resources/documentComment.md)|Update the properties of a [documentComment](../resources/documentcomment.md) object.|
|[List replies](../api/documentcomment-list-replies.md)|[documentCommentReply](../resources/documentCommentReply.md) collection|Get the documentCommentReplies from the replies navigation property.|
|[Add replies](../api/documentcomment-post-replies.md)|[documentCommentReply](../resources/documentCommentReply.md)|Add replies by posting to the replies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|replies|[documentCommentReply](../resources/documentCommentReply.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentComment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentComment",
  "id": "String (identifier)",
  "content": "String"
}
```

