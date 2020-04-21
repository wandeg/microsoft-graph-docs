---
title: "workbookCommentReply resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookCommentReply resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookCommentReply](../api/workbookcommentreply-get.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Read properties and relationships of a [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[Update workbookCommentReply](../api/workbookcommentreply-update.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Update the properties of a [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[List replies](../api/workbookcomment-list-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md) collection|Get the workbookCommentReplies from the replies navigation property.|
|[Create replies](../api/workbookcomment-post-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Create a new replies object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

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

