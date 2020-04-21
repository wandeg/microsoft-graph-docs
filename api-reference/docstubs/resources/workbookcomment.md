---
title: "workbookComment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookComment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookComment](../api/workbookcomment-get.md)|[workbookComment](../resources/workbookcomment.md)|Read properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.|
|[Update workbookComment](../api/workbookcomment-update.md)|[workbookComment](../resources/workbookcomment.md)|Update the properties of a [workbookComment](../resources/workbookcomment.md) object.|
|[List replies](../api/workbookcomment-list-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md) collection|Get the workbookCommentReplies from the replies navigation property.|
|[Create replies](../api/workbookcomment-post-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Create a new replies object.|
|[Delete replies](../api/workbookcomment-delete-replies.md)|None|Delete a replies object.|
|[Update replies](../api/workbookcomment-update-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Update the properties of a replies object.|
|[Get workbookCommentReply](../api/workbookcommentreply-get.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Read properties and relationships of a [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[List comments](../api/workbook-list-comments.md)|[workbookComment](../resources/workbookcomment.md) collection|Get the workbookComments from the comments navigation property.|
|[Create comments](../api/workbook-post-comments.md)|[workbookComment](../resources/workbookcomment.md)|Create a new comments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|replies|[workbookCommentReply](../resources/workbookcommentreply.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookComment",
  "id": "String (identifier)",
  "content": "String",
  "contentType": "String"
}
```

