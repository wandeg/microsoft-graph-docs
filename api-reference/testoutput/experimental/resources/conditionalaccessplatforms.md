---
title: "conditionalAccessPlatforms resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessPlatforms resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludePlatforms|Enumeration collection||
|includePlatforms|Enumeration collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessPlatforms",
  "includePlatforms": [
    "String"
  ],
  "excludePlatforms": [
    "String"
  ]
}
```

