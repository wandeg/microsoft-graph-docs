---
title: "OverlapInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# OverlapInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|detail|[OverlapInfoDetail](../resources/overlapinfodetail.md)||
|overlapType|Enumeration| Possible values are: `BOTH_CURRENT_VIEWER_STARTED_FIRST`, `BOTH_CURRENT_VIEWEE_STARTED_FIRST`, `BOTH_CURRENT_STARTED_IN_SAME_MONTH`, `NOT_BOTH_CURRENT_NO_OVERLAP_VIEWER_STARTED_FIRST`, `NOT_BOTH_CURRENT_NO_OVERLAP_VIEWEE_STARTED_FIRST`, `NOT_BOTH_CURRENT_OVERLAP`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.OverlapInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.OverlapInfo",
  "detail": {
    "@odata.type": "microsoft.graph.OverlapInfoDetail",
    "dateRange": {
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
    "duration": {
      "@odata.type": "microsoft.graph.Duration",
      "numDays": 1024,
      "numMonths": 1024,
      "numYears": 1024
    }
  },
  "overlapType": "String"
}
```

