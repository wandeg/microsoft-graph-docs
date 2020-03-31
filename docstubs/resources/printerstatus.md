---
title: "printerStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerStatus resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|processingState|Enumeration| Possible values are: `unknown`, `idle`, `processing`, `stopped`, `unknownFutureValue`.|
|processingStateDescription|String||
|processingStateReasons|Enumeration collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

