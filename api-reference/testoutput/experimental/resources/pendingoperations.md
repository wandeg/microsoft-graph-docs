---
title: "pendingOperations resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# pendingOperations resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|pendingContentUpdate|[pendingContentUpdate](../resources/pendingContentUpdate.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pendingOperations"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pendingOperations",
  "pendingContentUpdate": {
    "@odata.type": "microsoft.graph.pendingContentUpdate",
    "queuedDateTime": "String (timestamp)"
  }
}
```

