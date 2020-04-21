---
title: "daylightTimeZoneOffset resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# daylightTimeZoneOffset resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|daylightBias|Int32|**TODO: Add Description**|
|dayOccurrence|Int32|**TODO: Add Description** Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|dayOfWeek|dayOfWeek|**TODO: Add Description** Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md). Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|month|Int32|**TODO: Add Description** Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|time|TimeOfDay|**TODO: Add Description** Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|
|year|Int32|**TODO: Add Description** Inherited from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.daylightTimeZoneOffset",
  "time": "String (time of day)",
  "dayOccurrence": 1024,
  "dayOfWeek": "String",
  "month": 1024,
  "year": 1024,
  "daylightBias": 1024
}
```

