---
title: "outlookTaskFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# outlookTaskFolder resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md)|[outlookTaskFolder](../resources/outlookTaskFolder.md)|Read properties and relationships of the [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[Delete outlookTaskFolder](../api/outlooktaskfolder-delete.md)|None|Deletes a [outlookTaskFolder](../resources/outlooktaskfolder.md).|
|[Update outlookTaskFolder](../api/outlooktaskfolder-update.md)|[outlookTaskFolder](../resources/outlookTaskFolder.md)|Update the properties of a [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[List tasks](../api/outlooktaskfolder-list-tasks.md)|[outlookTask](../resources/outlookTask.md) collection|Get the outlookTasks from the tasks navigation property.|
|[Add tasks](../api/outlooktaskfolder-post-tasks.md)|[outlookTask](../resources/outlookTask.md)|Add tasks by posting to the tasks collection.|
|[List singleValueExtendedProperties](../api/outlooktaskfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/outlooktaskfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/outlooktaskfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/outlooktaskfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|

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
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection||
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection||
|tasks|[outlookTask](../resources/outlookTask.md) collection||

## JSON Representation
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

