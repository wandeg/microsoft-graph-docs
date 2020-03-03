---
title: "updateWindow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# updateWindow resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|updateWindowEndTime|TimeOfDay||
|updateWindowStartTime|TimeOfDay||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindow",
  "updateWindowStartTime": "String (time of day)",
  "updateWindowEndTime": "String (time of day)"
}
```

