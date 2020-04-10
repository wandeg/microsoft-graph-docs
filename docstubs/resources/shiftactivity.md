---
title: "shiftActivity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# shiftActivity resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|endDateTime|DateTimeOffset||
|isPaid|Boolean||
|startDateTime|DateTimeOffset||
|theme|Enumeration| Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

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

