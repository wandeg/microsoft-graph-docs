---
title: "outlookTaskFolder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# outlookTaskFolder resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Read the properties and relationships of an [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[Update outlookTaskFolder](../api/outlooktaskfolder-update.md)|[outlookTaskFolder](../resources/outlooktaskfolder.md)|Update the properties of an [outlookTaskFolder](../resources/outlooktaskfolder.md) object.|
|[List tasks](../api/outlooktaskfolder-list-tasks.md)|[outlookTask](../resources/outlooktask.md) collection|Get the outlookTasks from the tasks navigation property.|
|[Create tasks](../api/outlooktaskfolder-post-tasks.md)|[outlookTask](../resources/outlooktask.md)|Create a new tasks object.|
|[Delete tasks](../api/outlooktaskfolder-delete-tasks.md)|None|Delete a [outlookTask](../resources/outlooktask.md) object.|
|[Update tasks](../api/outlooktaskfolder-update-tasks.md)|[outlookTask](../resources/outlooktask.md)|Update the properties of a tasks object.|
|[Get outlookTask](../api/outlooktask-get.md)|[outlookTask](../resources/outlooktask.md)|Read the properties and relationships of an [outlookTask](../resources/outlooktask.md) object.|
|[List singleValueExtendedProperties](../api/outlooktaskfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/outlooktaskfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/outlooktaskfolder-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/outlooktaskfolder-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/outlooktaskfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/outlooktaskfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/outlooktaskfolder-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/outlooktaskfolder-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeKey|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefaultFolder|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|parentGroupKey|Guid|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|tasks|[outlookTask](../resources/outlooktask.md) collection|**TODO: Add Description**|

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

