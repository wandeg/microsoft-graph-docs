---
title: "filter resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# filter resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryFilterGroups|[filterGroup](../resources/filtergroup.md) collection|**TODO: Add Description**|
|groups|[filterGroup](../resources/filtergroup.md) collection|**TODO: Add Description**|
|inputFilterGroups|[filterGroup](../resources/filtergroup.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

