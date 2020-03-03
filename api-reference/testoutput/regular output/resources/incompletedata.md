---
title: "incompleteData resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# incompleteData resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|missingDataBeforeDateTime|DateTimeOffset||
|wasThrottled|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.incompleteData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incompleteData",
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": true
}
```

