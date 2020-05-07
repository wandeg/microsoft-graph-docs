---
title: "workbookComment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookComment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List replies](../api/workbookcomment-list-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md) collection|Get the workbookCommentReplies from the replies navigation property.|
|[Create replies](../api/workbookcomment-post-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Create a new replies object.|
|[Delete replies](../api/workbookcomment-delete-replies.md)|None|Delete a [workbookCommentReply](../resources/workbookcommentreply.md) object.|
|[Update replies](../api/workbookcomment-update-replies.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Update the properties of a replies object.|
|[Get workbookCommentReply](../api/workbookcommentreply-get.md)|[workbookCommentReply](../resources/workbookcommentreply.md)|Read the properties and relationships of a [workbookCommentReply](../resources/workbookcommentreply.md) object.|
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
The following is a JSON representation of the resource.
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

