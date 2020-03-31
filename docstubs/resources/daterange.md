---
title: "DateRange resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DateRange resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|end|[Date](../resources/date.md)||
|start|[Date](../resources/date.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.DateRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DateRange",
  "start": {
    "@odata.type": "microsoft.graph.Date",
    "day": 1024,
    "month": 1024,
    "year": 1024
  },
  "end": {
    "@odata.type": "microsoft.graph.Date"
  }
}
```

