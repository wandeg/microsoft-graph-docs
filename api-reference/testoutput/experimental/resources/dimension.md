---
title: "dimension resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dimension resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List dimensions](../api/dimension-list.md)|[dimension](../resources/dimension.md) collection|List properties and relationships of the [dimension](../resources/dimension.md) objects.|
|[Get dimension](../api/dimension-get.md)|[dimension](../resources/dimension.md)|Read properties and relationships of the [dimension](../resources/dimension.md) object.|
|[Create dimension](../api/dimension-create.md)|[dimension](../resources/dimension.md)|Create a new [dimension](../resources/dimension.md) object.|
|[Delete dimension](../api/dimension-delete.md)|None|Deletes a [dimension](../resources/dimension.md).|
|[Update dimension](../api/dimension-update.md)|[dimension](../resources/dimension.md)|Update the properties of a [dimension](../resources/dimension.md) object.|
|[List dimensionValues](../api/dimension-list-dimensionvalues.md)|[dimensionValue](../resources/dimensionvalue.md) collection|Get the dimensionValues from the dimensionValues navigation property.|
|[Add dimensionValues](../api/dimension-post-dimensionvalues.md)|[dimensionValue](../resources/dimensionvalue.md)|Add dimensionValues by posting to the dimensionValues collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dimensionValues|[dimensionValue](../resources/dimensionvalue.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dimension",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dimension",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

