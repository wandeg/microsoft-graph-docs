---
title: "printerStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|processingState|printerProcessingState|**TODO: Add Description**. Possible values are: `unknown`, `idle`, `processing`, `stopped`, `unknownFutureValue`.|
|processingStateDescription|String|**TODO: Add Description**|
|processingStateReasons|printerProcessingStateReason collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "processingState": "String",
  "processingStateReasons": [
    "String"
  ],
  "processingStateDescription": "String"
}
```

