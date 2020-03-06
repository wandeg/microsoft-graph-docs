---
title: "contentClassification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# contentClassification resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|confidence|Int32||
|matches|[matchLocation](../resources/matchlocation.md) collection||
|sensitiveTypeId|String||
|uniqueCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentClassification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentClassification",
  "sensitiveTypeId": "String",
  "uniqueCount": 1024,
  "confidence": 1024,
  "matches": [
    {
      "@odata.type": "microsoft.graph.matchLocation",
      "length": 1024,
      "offset": 1024
    }
  ]
}
```

