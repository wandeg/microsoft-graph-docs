---
title: "shiftItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# shiftItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [scheduleEntity](../resources/scheduleentity.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[shiftActivity](../resources/shiftactivity.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|notes|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md)|
|theme|scheduleEntityTheme|**TODO: Add Description** Inherited from [scheduleEntity](../resources/scheduleentity.md). Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
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

