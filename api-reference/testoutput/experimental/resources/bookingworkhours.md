---
title: "bookingWorkHours resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingWorkHours resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|day|Enumeration|The day of the week represented by this instance. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|timeSlots|[bookingWorkTimeSlot](../resources/bookingworktimeslot.md) collection|A list of start/end times during a day.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingWorkHours"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingWorkHours",
  "day": "String",
  "timeSlots": [
    {
      "@odata.type": "microsoft.graph.bookingWorkTimeSlot",
      "start": "String (time of day)",
      "end": "String (time of day)"
    }
  ]
}
```

