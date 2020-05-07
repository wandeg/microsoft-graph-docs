---
title: "printJobStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printJobStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acquiredByPrinter|Boolean|**TODO: Add Description**|
|processingState|printJobProcessingState|**TODO: Add Description**. Possible values are: `unknown`, `pending`, `pendingHeld`, `processing`, `paused`, `stopped`, `completed`, `canceled`, `aborted`.|
|processingStateDescription|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "acquiredByPrinter": "Boolean"
}
```

