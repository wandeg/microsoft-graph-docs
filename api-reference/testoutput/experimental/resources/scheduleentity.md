---
title: "scheduleEntity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# scheduleEntity resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|theme|Enumeration|. Possible values are: `white`, `blue`, `green`, `purple`, `pink`, `yellow`, `gray`, `darkBlue`, `darkGreen`, `darkPurple`, `darkPink`, `darkYellow`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scheduleEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleEntity",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String"
}
```

