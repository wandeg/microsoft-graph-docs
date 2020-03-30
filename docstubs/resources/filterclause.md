---
title: "filterClause resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# filterClause resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|operatorName|String||
|sourceOperandName|String||
|targetOperand|[filterOperand](../resources/filteroperand.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.filterClause"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filterClause",
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {
    "@odata.type": "microsoft.graph.filterOperand",
    "values": [
      "String"
    ]
  }
}
```

