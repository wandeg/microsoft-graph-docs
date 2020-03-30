---
title: "synchronizationProgress resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationProgress resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedUnits|Int64||
|progressObservationDateTime|DateTimeOffset||
|totalUnits|Int64||
|units|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationProgress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationProgress",
  "completedUnits": 1024,
  "progressObservationDateTime": "String (timestamp)",
  "totalUnits": 1024,
  "units": "String"
}
```

