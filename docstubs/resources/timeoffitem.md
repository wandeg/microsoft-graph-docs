---
title: "timeOffItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# timeOffItem resource type


Namespace: microsoft.graph




Inherits from [scheduleEntity](../resources/scheduleentity.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|startDateTime|DateTimeOffset| Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|theme|Enumeration| Inherited from [scheduleEntity](../resources/scheduleentity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|
|timeOffReasonId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeOffItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeOffItem",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "timeOffReasonId": "String"
}
```

