---
title: "filterGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# filterGroup resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|clauses|[filterClause](../resources/filterclause.md) collection||
|name|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.filterGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filterGroup",
  "clauses": [
    {
      "@odata.type": "microsoft.graph.filterClause",
      "operatorName": "String",
      "sourceOperandName": "String",
      "targetOperand": {
        "@odata.type": "microsoft.graph.filterOperand",
        "values": [
          "String"
        ]
      }
    }
  ],
  "name": "String"
}
```

