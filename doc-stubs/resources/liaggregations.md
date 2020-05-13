---
title: "LIAggregations resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIAggregations resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregationField|String|**TODO: Add Description**|
|buckets|[LIAggregationBucket](../resources/liaggregationbucket.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.LIAggregationBucket"
    }
  ]
}
```

