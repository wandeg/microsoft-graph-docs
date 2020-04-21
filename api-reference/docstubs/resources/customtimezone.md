---
title: "customTimeZone resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# customTimeZone resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [timeZoneBase](../resources/timezonebase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bias|Int32|**TODO: Add Description**|
|daylightOffset|[daylightTimeZoneOffset](../resources/daylighttimezoneoffset.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [timeZoneBase](../resources/timezonebase.md)|
|standardOffset|[standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customTimeZone"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customTimeZone",
  "name": "String",
  "bias": 1024,
  "standardOffset": {
    "@odata.type": "microsoft.graph.standardTimeZoneOffset",
    "time": "String (time of day)",
    "dayOccurrence": 1024,
    "dayOfWeek": "String",
    "month": 1024,
    "year": 1024
  },
  "daylightOffset": {
    "@odata.type": "microsoft.graph.daylightTimeZoneOffset",
    "daylightBias": 1024
  }
}
```

