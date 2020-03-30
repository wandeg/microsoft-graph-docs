---
title: "PositionChange resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# PositionChange resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|newPosition|[Position](../resources/position.md)||
|oldPosition|[Position](../resources/position.md)||
|positionChangeType|Enumeration| Possible values are: `PROMOTION`, `COMPANY_CHANGE`, `POSITION_CHANGE`, `ADDITIONAL_POSITION`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.PositionChange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.PositionChange",
  "newPosition": {
    "@odata.type": "microsoft.graph.Position",
    "name": "String",
    "logo": "String",
    "url": "String",
    "location": "String",
    "title": "String",
    "startEndDate": {
      "@odata.type": "microsoft.graph.DateRange",
      "start": {
        "@odata.type": "microsoft.graph.Date",
        "day": 1024,
        "month": 1024,
        "year": 1024
      },
      "end": {
        "@odata.type": "microsoft.graph.Date"
      }
    },
    "description": "String"
  },
  "oldPosition": {
    "@odata.type": "microsoft.graph.Position"
  },
  "positionChangeType": "String"
}
```

