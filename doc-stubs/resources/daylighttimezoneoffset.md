---
title: "daylightTimeZoneOffset resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# daylightTimeZoneOffset resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [standardTimeZoneOffset](../resources/standardtimezoneoffset.md).

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
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.daylightTimeZoneOffset",
  "time": "String (time of day)",
  "dayOccurrence": "Integer",
  "dayOfWeek": "String",
  "month": "Integer",
  "year": "Integer",
  "daylightBias": "Integer"
}
```

