---
title: "windowsKioskForceUpdateSchedule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsKioskForceUpdateSchedule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|dayofMonth|Int32||
|dayofWeek|Enumeration| Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|recurrence|Enumeration| Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|runImmediatelyIfAfterStartDateTime|Boolean||
|startDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```

