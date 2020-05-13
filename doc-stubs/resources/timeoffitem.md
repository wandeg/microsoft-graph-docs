---
title: "timeOffItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# timeOffItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [scheduleEntity](../resources/scheduleentity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|theme|scheduleEntityTheme|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|
|timeOffReasonId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

