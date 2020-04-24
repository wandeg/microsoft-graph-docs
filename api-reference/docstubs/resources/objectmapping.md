---
title: "objectMapping resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# objectMapping resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributeMappings|[attributeMapping](../resources/attributemapping.md) collection|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|flowTypes|objectFlowTypes|**TODO: Add Description**. Possible values are: `None`, `Add`, `Update`, `Delete`.|
|metadata|[metadataEntry](../resources/metadataentry.md) collection|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|scope|[filter](../resources/filter.md)|**TODO: Add Description**|
|sourceObjectName|String|**TODO: Add Description**|
|targetObjectName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

