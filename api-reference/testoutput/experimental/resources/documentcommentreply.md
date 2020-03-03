---
title: "documentCommentReply resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# documentCommentReply resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get documentCommentReply](../api/documentcommentreply-get.md)|[documentCommentReply](../resources/documentCommentReply.md)|Read properties and relationships of the [documentCommentReply](../resources/documentcommentreply.md) object.|
|[Delete documentCommentReply](../api/documentcommentreply-delete.md)|None|Deletes a [documentCommentReply](../resources/documentcommentreply.md).|
|[Update documentCommentReply](../api/documentcommentreply-update.md)|[documentCommentReply](../resources/documentCommentReply.md)|Update the properties of a [documentCommentReply](../resources/documentcommentreply.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.documentCommentReply",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentCommentReply",
  "id": "String (identifier)",
  "content": "String"
}
```

