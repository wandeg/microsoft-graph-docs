---
title: "workingHours resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workingHours resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|daysOfWeek|dayOfWeek collection|**TODO: Add Description**|
|endTime|TimeOfDay|**TODO: Add Description**|
|startTime|TimeOfDay|**TODO: Add Description**|
|timeZone|[timeZoneBase](../resources/timezonebase.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workingHours"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workingHours",
  "daysOfWeek": [
    "String"
  ],
  "startTime": "String (time of day)",
  "endTime": "String (time of day)",
  "timeZone": {
    "@odata.type": "microsoft.graph.timeZoneBase"
  }
}
```

