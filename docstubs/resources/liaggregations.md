---
title: "LIAggregations resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIAggregations resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregationField|String||
|buckets|[LIAggregationBucket](../resources/liaggregationbucket.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIAggregations"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIAggregations",
  "aggregationField": "String",
  "buckets": [
    {
      "@odata.type": "microsoft.graph.LIAggregationBucket",
      "id": "String",
      "term": "String",
      "count": 1024
    }
  ]
}
```

