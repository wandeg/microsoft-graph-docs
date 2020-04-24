---
title: "schema resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# schema resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get schema](../api/schema-get.md)|[schema](../resources/schema.md)|Read the properties and relationships of a [schema](../resources/schema.md) object.|
|[Update schema](../api/schema-update.md)|[schema](../resources/schema.md)|Update the properties of a [schema](../resources/schema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|baseType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|properties|[property](../resources/property.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

