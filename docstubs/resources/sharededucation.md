---
title: "SharedEducation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SharedEducation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|location|String||
|logo|String||
|name|String||
|overlapInfo|[OverlapInfo](../resources/overlapinfo.md)||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SharedEducation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SharedEducation",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "overlapInfo": {
    "@odata.type": "microsoft.graph.OverlapInfo",
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
}
```

