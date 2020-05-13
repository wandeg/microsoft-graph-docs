---
title: "Result resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# Result resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[query](../api/result-query.md)|[Result](../resources/result.md) collection|**TODO: Add Description**|
|[query](../api/result-query.md)|[Result](../resources/result.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregations|[LIAggregations](../resources/liaggregations.md) collection|**TODO: Add Description**|
|entities|[ResultEntities](../resources/resultentities.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|metadata|[Metadata](../resources/metadata.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

