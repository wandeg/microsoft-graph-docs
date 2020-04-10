---
title: "searchHitsContainer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# searchHitsContainer resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hits|[searchHit](../resources/searchhit.md) collection||
|moreResultsAvailable|Boolean||
|total|Int32||

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

