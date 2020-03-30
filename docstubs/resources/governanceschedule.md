---
title: "governanceSchedule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceSchedule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|duration|Duration||
|endDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceSchedule",
  "type": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "String (duration)"
}
```

