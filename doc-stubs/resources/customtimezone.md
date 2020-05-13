---
title: "customTimeZone resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# customTimeZone resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [timeZoneBase](../resources/timezonebase.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bias|Int32|**TODO: Add Description**|
|daylightOffset|[daylightTimeZoneOffset](../resources/daylighttimezoneoffset.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description** Inherited from [timeZoneBase](../resources/timezonebase.md)|
|standardOffset|[standardTimeZoneOffset](../resources/standardtimezoneoffset.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customTimeZone"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customTimeZone",
  "name": "String",
  "bias": "Integer",
  "standardOffset": {
    "@odata.type": "microsoft.graph.standardTimeZoneOffset"
  },
  "daylightOffset": {
    "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
  }
}
```

