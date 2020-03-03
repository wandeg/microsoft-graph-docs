---
title: "outlookTaskGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# outlookTaskGroup resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookTaskGroup](../api/outlooktaskgroup-get.md)|[outlookTaskGroup](../resources/outlookTaskGroup.md)|Read properties and relationships of the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.|
|[Delete outlookTaskGroup](../api/outlooktaskgroup-delete.md)|None|Deletes a [outlookTaskGroup](../resources/outlooktaskgroup.md).|
|[Update outlookTaskGroup](../api/outlooktaskgroup-update.md)|[outlookTaskGroup](../resources/outlookTaskGroup.md)|Update the properties of a [outlookTaskGroup](../resources/outlooktaskgroup.md) object.|
|[List taskFolders](../api/outlooktaskgroup-list-taskfolders.md)|[outlookTaskFolder](../resources/outlookTaskFolder.md) collection|Get the outlookTaskFolders from the taskFolders navigation property.|
|[Add taskFolders](../api/outlooktaskgroup-post-taskfolders.md)|[outlookTaskFolder](../resources/outlookTaskFolder.md)|Add taskFolders by posting to the taskFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String||
|groupKey|Guid||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefaultGroup|Boolean||
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|taskFolders|[outlookTaskFolder](../resources/outlookTaskFolder.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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
  "isDefaultGroup": true,
  "name": "String",
  "groupKey": "Guid"
}
```

