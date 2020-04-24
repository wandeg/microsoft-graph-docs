---
title: "searchHitsContainer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# searchHitsContainer resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hits|[searchHit](../resources/searchhit.md) collection|**TODO: Add Description**|
|moreResultsAvailable|Boolean|**TODO: Add Description**|
|total|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchHitsContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchHitsContainer",
  "hits": [
    {
      "@odata.type": "microsoft.graph.searchHit",
      "_id": "String",
      "_score": 1024,
      "_sortField": "String",
      "_summary": "String",
      "_source": {
        "@odata.type": "#microsoft.graph.entity",
        "id": "String (identifier)"
      }
    }
  ],
  "total": 1024,
  "moreResultsAvailable": true
}
```

