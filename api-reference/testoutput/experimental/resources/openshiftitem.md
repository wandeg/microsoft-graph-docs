---
title: "openShiftItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# openShiftItem resource type




Inherits from [shiftItem](../resources/shiftItem.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[shiftActivity](../resources/shiftActivity.md) collection| Inherited from [shiftItem](../resources/shiftItem.md)|
|displayName|String| Inherited from [shiftItem](../resources/shiftItem.md)|
|endDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleEntity.md)|
|notes|String| Inherited from [shiftItem](../resources/shiftItem.md)|
|openSlotCount|Int32||
|startDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleEntity.md)|
|theme|Enumeration| Inherited from [scheduleEntity](../resources/scheduleEntity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

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

