---
title: "filterClause resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# filterClause resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|operatorName|String||
|sourceOperandName|String||
|targetOperand|[filterOperand](../resources/filterOperand.md)||

## Relationships
None

## JSON Representation
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

