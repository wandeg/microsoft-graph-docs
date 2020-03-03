---
title: "scheduleInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# scheduleInformation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityView|String||
|error|[freeBusyError](../resources/freeBusyError.md)||
|scheduleId|String||
|scheduleItems|[scheduleItem](../resources/scheduleItem.md) collection||
|workingHours|[workingHours](../resources/workingHours.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scheduleInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleInformation",
  "scheduleId": "String",
  "scheduleItems": [
    {
      "@odata.type": "microsoft.graph.scheduleItem",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone",
        "dateTime": "String",
        "timeZone": "String"
      },
      "end": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "isPrivate": true,
      "status": "String",
      "subject": "String",
      "location": "String"
    }
  ],
  "availabilityView": "String",
  "error": {
    "@odata.type": "microsoft.graph.freeBusyError",
    "message": "String",
    "responseCode": "String"
  },
  "workingHours": {
    "@odata.type": "microsoft.graph.workingHours",
    "daysOfWeek": [
      "String"
    ],
    "startTime": "String (time of day)",
    "endTime": "String (time of day)",
    "timeZone": {
      "@odata.type": "microsoft.graph.timeZoneBase",
      "name": "String"
    }
  }
}
```

