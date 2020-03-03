---
title: "documentComment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# documentComment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List documentComments](../api/documentcomment-list.md)|[documentComment](../resources/documentcomment.md) collection|List properties and relationships of the [documentComment](../resources/documentcomment.md) objects.|
|[Get documentComment](../api/documentcomment-get.md)|[documentComment](../resources/documentcomment.md)|Read properties and relationships of the [documentComment](../resources/documentcomment.md) object.|
|[Create documentComment](../api/documentcomment-create.md)|[documentComment](../resources/documentcomment.md)|Create a new [documentComment](../resources/documentcomment.md) object.|
|[Delete documentComment](../api/documentcomment-delete.md)|None|Deletes a [documentComment](../resources/documentcomment.md).|
|[Update documentComment](../api/documentcomment-update.md)|[documentComment](../resources/documentcomment.md)|Update the properties of a [documentComment](../resources/documentcomment.md) object.|
|[List replies](../api/documentcomment-list-replies.md)|[documentCommentReply](../resources/documentcommentreply.md) collection|Get the documentCommentReplies from the replies navigation property.|
|[Add replies](../api/documentcomment-post-replies.md)|[documentCommentReply](../resources/documentcommentreply.md)|Add replies by posting to the replies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|replies|[documentCommentReply](../resources/documentcommentreply.md) collection||

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

