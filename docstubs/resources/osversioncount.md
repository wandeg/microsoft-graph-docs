---
title: "osVersionCount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# osVersionCount resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceCount|Int32||
|lastUpdateDateTime|DateTimeOffset||
|osVersion|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```

