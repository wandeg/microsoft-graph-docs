---
title: "outlookTaskFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# outlookTaskFolder resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Read properties and relationships of the [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[Update outlookTaskFolder](../api/outlooktaskfolder-update.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Update the properties of a [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[List tasks](../api/outlooktaskfolder-list-tasks.md)|[outlookTask](../resources/outlooktask.md) collection|Get the outlookTasks from the tasks navigation property.|
|[Add tasks](../api/outlooktaskfolder-post-tasks.md)|[outlookTask](../resources/outlooktask.md)|Add tasks by posting to the tasks collection.|
|[List singleValueExtendedProperties](../api/outlooktaskfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/outlooktaskfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/outlooktaskfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/outlooktaskfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List taskFolders](../api/outlookuser-list-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md) collection|Get the outlookTaskFolders from the taskFolders navigation property.|
|[Add taskFolders](../api/outlookuser-post-taskfolders.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Add taskFolders by posting to the taskFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefaultFolder|Boolean||
|name|String||
|parentGroupKey|Guid||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection||
|tasks|[outlookTask](../resources/outlooktask.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "id": "String (identifier)",
  "changeKey": "String",
  "name": "String",
  "isDefaultFolder": true,
  "parentGroupKey": "Guid"
}
```

