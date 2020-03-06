---
title: "conditionalAccessApplications resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessApplications resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeApplications|String collection||
|includeApplications|String collection||
|includeUserActions|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessApplications",
  "includeApplications": [
    "String"
  ],
  "excludeApplications": [
    "String"
  ],
  "includeUserActions": [
    "String"
  ]
}
```

