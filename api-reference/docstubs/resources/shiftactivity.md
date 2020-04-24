---
title: "shiftActivity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# shiftActivity resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|isPaid|Boolean|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|theme|scheduleEntityTheme|**TODO: Add Description**. Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shiftActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shiftActivity",
  "isPaid": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "code": "String",
  "displayName": "String",
  "theme": "String"
}
```

