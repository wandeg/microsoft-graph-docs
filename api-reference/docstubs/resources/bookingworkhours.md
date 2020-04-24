---
title: "bookingWorkHours resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingWorkHours resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|day|dayOfWeek|The day of the week represented by this instance. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|timeSlots|[bookingWorkTimeSlot](../resources/bookingworktimeslot.md) collection|A list of start/end times during a day.|

## Relationships
None

## JSON representation
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

