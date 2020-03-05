---
title: "workbookCommentReply resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookCommentReply resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookCommentReplies](../api/workbookcommentreply-list.md)|[workbookCommentReply](../resources/workbookcommentreply.md) collection|List properties and relationships of the [workbookCommentReply](../resources/workbookcommentreply.md) objects.|
|[Get workbookCommentReply](../api/workbookcommentreply-get.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Read properties and relationships of the [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[Create workbookCommentReply](../api/workbookcommentreply-create.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[Delete workbookCommentReply](../api/workbookcommentreply-delete.md)|None|Deletes a [workbookCommentReply](../resources/workbookcommentreply.md).|
|[Update workbookCommentReply](../api/workbookcommentreply-update.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Update the properties of a [workbookCommentReply](../resources/workbookcommentreply.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String||
|contentType|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "id": "String (identifier)",
  "content": "String",
  "contentType": "String"
}
```

