---
title: "customUpdateTimeWindow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# customUpdateTimeWindow resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDay|Enumeration| Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|endTime|TimeOfDay||
|startDay|Enumeration| Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|startTime|TimeOfDay||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```

