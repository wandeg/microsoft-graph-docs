---
title: "searchResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# searchResponse resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|hitsContainers|[searchHitsContainer](../resources/searchhitscontainer.md) collection||
|searchTerms|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchResponse",
  "searchTerms": [
    "String"
  ],
  "hitsContainers": [
    {
      "@odata.type": "microsoft.graph.searchHitsContainer",
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
  ]
}
```

