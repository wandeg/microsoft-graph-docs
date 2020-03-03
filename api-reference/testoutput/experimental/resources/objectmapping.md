---
title: "objectMapping resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# objectMapping resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributeMappings|[attributeMapping](../resources/attributeMapping.md) collection||
|enabled|Boolean||
|flowTypes|Enumeration|. Possible values are: `None`, `Add`, `Update`, `Delete`.|
|metadata|[metadataEntry](../resources/metadataEntry.md) collection||
|name|String||
|scope|[filter](../resources/filter.md)||
|sourceObjectName|String||
|targetObjectName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.objectMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.objectMapping",
  "attributeMappings": [
    {
      "@odata.type": "microsoft.graph.attributeMapping",
      "defaultValue": "String",
      "exportMissingReferences": true,
      "flowBehavior": "String",
      "flowType": "String",
      "matchingPriority": 1024,
      "source": {
        "@odata.type": "microsoft.graph.attributeMappingSource",
        "expression": "String",
        "name": "String",
        "parameters": [
          {
            "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
            "key": "String",
            "value": {
              "@odata.type": "microsoft.graph.attributeMappingSource",
              "type": "String"
            }
          }
        ]
      },
      "targetAttributeName": "String"
    }
  ],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry",
      "value": "String"
    }
  ],
  "name": "String",
  "scope": {
    "@odata.type": "microsoft.graph.filter",
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
        ]
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
  },
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

