---
title: "conditionalAccessLocations resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessLocations resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeLocations|String collection||
|includeLocations|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessLocations"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessLocations",
  "includeLocations": [
    "String"
  ],
  "excludeLocations": [
    "String"
  ]
}
```

