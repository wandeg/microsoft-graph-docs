---
title: "printJobStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printJobStatus resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|acquiredByPrinter|Boolean||
|processingState|Enumeration| Possible values are: `unknown`, `pending`, `pendingHeld`, `processing`, `paused`, `stopped`, `completed`, `canceled`, `aborted`.|
|processingStateDescription|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "processingState": "String",
  "processingStateDescription": "String",
  "acquiredByPrinter": true
}
```

