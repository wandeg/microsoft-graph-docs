---
title: "filter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# filter resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryFilterGroups|[filterGroup](../resources/filterGroup.md) collection||
|groups|[filterGroup](../resources/filterGroup.md) collection||
|inputFilterGroups|[filterGroup](../resources/filterGroup.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.filter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filter",
  "groups": [
    {
      "@odata.type": "microsoft.graph.filterGroup",
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
  ],
  "inputFilterGroups": [
    {
      "@odata.type": "microsoft.graph.filterGroup"
    }
  ],
  "categoryFilterGroups": [
    {
      "@odata.type": "microsoft.graph.filterGroup"
    }
  ]
}
```

