---
title: "shiftAvailability resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# shiftAvailability resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|recurrence|[patternedRecurrence](../resources/patternedRecurrence.md)||
|timeSlots|[timeRange](../resources/timeRange.md) collection||
|timeZone|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shiftAvailability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shiftAvailability",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 1024,
      "month": 1024,
      "dayOfMonth": 1024,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "String",
      "numberOfOccurrences": 1024
    }
  },
  "timeZone": "String",
  "timeSlots": [
    {
      "@odata.type": "microsoft.graph.timeRange",
      "startTime": "String (time of day)",
      "endTime": "String (time of day)"
    }
  ]
}
```

