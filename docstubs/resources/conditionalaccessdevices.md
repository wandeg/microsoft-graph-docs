---
title: "conditionalAccessDevices resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# conditionalAccessDevices resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeDeviceStates|String collection||
|includeDeviceStates|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessDevices"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessDevices",
  "includeDeviceStates": [
    "String"
  ],
  "excludeDeviceStates": [
    "String"
  ]
}
```

