---
title: "scheduleInformation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# scheduleInformation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityView|String|**TODO: Add Description**|
|error|[freeBusyError](../resources/freebusyerror.md)|**TODO: Add Description**|
|scheduleId|String|**TODO: Add Description**|
|scheduleItems|[scheduleItem](../resources/scheduleitem.md) collection|**TODO: Add Description**|
|workingHours|[workingHours](../resources/workinghours.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

