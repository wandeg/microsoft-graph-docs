---
title: "outlookTaskGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outlookTaskGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List taskFolders](../api/outlooktaskgroup-list-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|Get the outlookTaskFolders from the taskFolders navigation property.|
|[Create taskFolders](../api/outlooktaskgroup-post-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Create a new taskFolders object.|
|[Delete taskFolders](../api/outlooktaskgroup-delete-taskfolders.md)|None|Delete a [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[Update taskFolders](../api/outlooktaskgroup-update-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Update the properties of a taskFolders object.|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Read the properties and relationships of an [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[List taskGroups](../api/outlookuser-list-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md) collection|Get the outlookTaskGroups from the taskGroups navigation property.|
|[Create taskGroups](../api/outlookuser-post-taskgroups.md)|[outlookTaskGroup](../resources/outlooktaskgroup.md)|Create a new taskGroups object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String|**TODO: Add Description**|
|groupKey|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefaultGroup|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|taskFolders|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "id": "String (identifier)",
  "changeKey": "String",
  "isDefaultGroup": "Boolean",
  "name": "String",
  "groupKey": "Guid"
}
```

