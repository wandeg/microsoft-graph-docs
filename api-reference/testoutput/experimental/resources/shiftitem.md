---
title: "shiftItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# shiftItem resource type


Namespace: microsoft.graph




Inherits from [scheduleEntity](../resources/scheduleentity.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[shiftActivity](../resources/shiftactivity.md) collection||
|displayName|String||
|endDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|notes|String||
|startDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|theme|Enumeration| Inherited from [scheduleEntity](../resources/scheduleentity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shiftItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shiftItem",
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
  ]
}
```

