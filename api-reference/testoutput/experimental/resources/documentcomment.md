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
|[Get documentComment](../api/documentcomment-get.md)|[documentComment](../resources/documentcomment.md)|Read properties and relationships of the [documentComment](../resources/documentcomment.md) object.|
|[Update documentComment](../api/documentcomment-update.md)|[documentComment](../resources/documentcomment.md)|Update the properties of a [documentComment](../resources/documentcomment.md) object.|
|[List replies](../api/documentcomment-list-replies.md)|[documentCommentReply](../resources/documentcommentreply.md) collection|Get the documentCommentReplies from the replies navigation property.|
|[Add replies](../api/documentcomment-post-replies.md)|[documentCommentReply](../resources/documentcommentreply.md)|Add replies by posting to the replies collection.|
|[List comments](../api/document-list-comments.md)|[documentComment](../resources/documentcomment.md) collection|Get the documentComments from the comments navigation property.|
|[Add comments](../api/document-post-comments.md)|[documentComment](../resources/documentcomment.md)|Add comments by posting to the comments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|replies|[documentCommentReply](../resources/documentcommentreply.md) collection||

## JSON representation
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

