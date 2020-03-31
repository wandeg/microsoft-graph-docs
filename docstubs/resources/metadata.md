---
title: "Metadata resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Metadata resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|searchMatches|[SearchMatch](../resources/searchmatch.md) collection||
|total|Int64||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Metadata"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Metadata",
  "total": 1024,
  "searchMatches": [
    {
      "@odata.type": "microsoft.graph.SearchMatch",
      "id": "String",
      "matchInfo": [
        {
          "@odata.type": "microsoft.graph.LIQueryTermMatchInfo",
          "fieldName": "String"
        }
      ]
    }
  ]
}
```

