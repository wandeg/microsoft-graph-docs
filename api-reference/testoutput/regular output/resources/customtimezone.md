---
title: "customTimeZone resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# customTimeZone resource type




Inherits from [timeZoneBase](../resources/timeZoneBase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bias|Int32||
|daylightOffset|[daylightTimeZoneOffset](../resources/daylightTimeZoneOffset.md)||
|name|String| Inherited from [timeZoneBase](../resources/timeZoneBase.md)|
|standardOffset|[standardTimeZoneOffset](../resources/standardTimeZoneOffset.md)||

## Relationships
None

## JSON Representation
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

