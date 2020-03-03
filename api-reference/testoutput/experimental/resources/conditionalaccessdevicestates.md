---
title: "conditionalAccessDeviceStates resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessDeviceStates resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeStates|String collection||
|includeStates|String collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessDeviceStates",
  "includeStates": [
    "String"
  ],
  "excludeStates": [
    "String"
  ]
}
```

