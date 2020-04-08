---
title: "filterOperatorSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# filterOperatorSchema resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List filterOperatorSchemas](../api/filteroperatorschema-list.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection|List properties and relationships of the [filterOperatorSchema](../resources/filteroperatorschema.md) objects.|
|[Get filterOperatorSchema](../api/filteroperatorschema-get.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Read properties and relationships of the [filterOperatorSchema](../resources/filteroperatorschema.md) object.|
|[Create filterOperatorSchema](../api/filteroperatorschema-post-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Create a new [filterOperatorSchema](../resources/filteroperatorschema.md) object.|
|[Delete filterOperatorSchema](../api/filteroperatorschema-delete.md)|None|Deletes a [filterOperatorSchema](../resources/filteroperatorschema.md).|
|[Update filterOperatorSchema](../api/filteroperatorschema-update.md)|[filterOperatorSchema](../resources/filteroperatorschema.md)|Update the properties of a [filterOperatorSchema](../resources/filteroperatorschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|arity|Enumeration| Possible values are: `Binary`, `Unary`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|multivaluedComparisonType|Enumeration| Possible values are: `All`, `Any`.|
|supportedAttributeTypes|Enumeration collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "id": "String (identifier)",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```

