---
title: "singleValueLegacyExtendedProperty resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# singleValueLegacyExtendedProperty resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List singleValueLegacyExtendedProperties](../api/singlevaluelegacyextendedproperty-list.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|List properties and relationships of the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read properties and relationships of the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Create singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-create.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Delete singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-delete.md)|None|Deletes a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).|
|[Update singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-update.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
  "id": "String (identifier)",
  "value": "String"
}
```

