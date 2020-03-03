---
title: "openShiftItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# openShiftItem resource type


Namespace: microsoft.graph




Inherits from [shiftItem](../resources/shiftitem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[shiftActivity](../resources/shiftactivity.md) collection| Inherited from [shiftItem](../resources/shiftitem.md)|
|displayName|String| Inherited from [shiftItem](../resources/shiftitem.md)|
|endDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|notes|String| Inherited from [shiftItem](../resources/shiftitem.md)|
|openSlotCount|Int32||
|startDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|theme|Enumeration| Inherited from [scheduleEntity](../resources/scheduleentity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openShiftItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.openShiftItem",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "displayName": "String",
  "notes": "String",
  "activities": [
    {
      "@odata.type": "microsoft.graph.shiftActivity",
      "isPaid": true,
      "code": "String"
    }
  ],
  "openSlotCount": 1024
}
```

