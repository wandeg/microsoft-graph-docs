---
title: "attributeMappingFunctionSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# attributeMappingFunctionSchema resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List attributeMappingFunctionSchemas](../api/attributemappingfunctionschema-list.md)|[attributeMappingFunctionSchema](../resources/attributeMappingFunctionSchema.md) collection|List properties and relationships of the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) objects.|
|[Get attributeMappingFunctionSchema](../api/attributemappingfunctionschema-get.md)|[attributeMappingFunctionSchema](../resources/attributeMappingFunctionSchema.md)|Read properties and relationships of the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|
|[Create attributeMappingFunctionSchema](../api/attributemappingfunctionschema-post-functions.md)|[attributeMappingFunctionSchema](../resources/attributeMappingFunctionSchema.md)|Create a new [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|
|[Delete attributeMappingFunctionSchema](../api/attributemappingfunctionschema-delete.md)|None|Deletes a [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md).|
|[Update attributeMappingFunctionSchema](../api/attributemappingfunctionschema-update.md)|[attributeMappingFunctionSchema](../resources/attributeMappingFunctionSchema.md)|Update the properties of a [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parameters|[attributeMappingParameterSchema](../resources/attributeMappingParameterSchema.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
  "id": "String (identifier)",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
    }
  ]
}
```

