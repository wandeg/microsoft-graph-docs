---
title: "failureInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# failureInfo resource type


Namespace: microsoft.graph.callRecords



## Properties
|Property|Type|Description|
|:---|:---|:---|
|reason|String||
|stage|Enumeration|. Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.failureInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.failureInfo",
  "stage": "String",
  "reason": "String"
}
```

