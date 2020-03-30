---
title: "Result resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Result resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List Results](../api/result-list.md)|[Result](../resources/result.md) collection|List properties and relationships of the [Result](../resources/result.md) objects.|
|[Get Result](../api/result-get.md)|[Result](../resources/result.md)|Read properties and relationships of the [Result](../resources/result.md) object.|
|[Create Result](../api/result-post-graph.md)|[Result](../resources/result.md)|Create a new [Result](../resources/result.md) object.|
|[Delete Result](../api/result-delete.md)|None|Deletes a [Result](../resources/result.md).|
|[Update Result](../api/result-update.md)|[Result](../resources/result.md)|Update the properties of a [Result](../resources/result.md) object.|
|[query](../api/result-query.md)|[Result](../resources/result.md) collection||
|[query](../api/result-query.md)|[Result](../resources/result.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregations|[LIAggregations](../resources/liaggregations.md) collection||
|entities|[ResultEntities](../resources/resultentities.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|metadata|[Metadata](../resources/metadata.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.Result",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Result",
  "id": "String (identifier)",
  "entities": {
    "@odata.type": "microsoft.graph.ResultEntities"
  },
  "aggregations": [
    {
      "@odata.type": "microsoft.graph.LIAggregations"
    }
  ],
  "metadata": {
    "@odata.type": "microsoft.graph.Metadata"
  }
}
```

