---
title: "conditionalAccessUsers resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessUsers resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroups|String collection||
|excludeRoles|String collection||
|excludeUsers|String collection||
|includeGroups|String collection||
|includeRoles|String collection||
|includeUsers|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessUsers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessUsers",
  "includeUsers": [
    "String"
  ],
  "excludeUsers": [
    "String"
  ],
  "includeGroups": [
    "String"
  ],
  "excludeGroups": [
    "String"
  ],
  "includeRoles": [
    "String"
  ],
  "excludeRoles": [
    "String"
  ]
}
```

