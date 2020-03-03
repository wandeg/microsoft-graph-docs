---
title: "schema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# schema resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List schemas](../api/schema-list.md)|[schema](../resources/schema.md) collection|List properties and relationships of the [schema](../resources/schema.md) objects.|
|[Get schema](../api/schema-get.md)|[schema](../resources/schema.md)|Read properties and relationships of the [schema](../resources/schema.md) object.|
|[Create schema](../api/schema-create.md)|[schema](../resources/schema.md)|Create a new [schema](../resources/schema.md) object.|
|[Delete schema](../api/schema-delete.md)|None|Deletes a [schema](../resources/schema.md).|
|[Update schema](../api/schema-update.md)|[schema](../resources/schema.md)|Update the properties of a [schema](../resources/schema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|baseType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|properties|[property](../resources/property.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.schema",
  "id": "String (identifier)",
  "baseType": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.property"
    }
  ]
}
```

