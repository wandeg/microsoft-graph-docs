---
title: "synchronizationRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationRule resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|editable|Boolean||
|id|String||
|metadata|[stringKeyStringValuePair](../resources/stringkeystringvaluepair.md) collection||
|name|String||
|objectMappings|[objectMapping](../resources/objectmapping.md) collection||
|priority|Int32||
|sourceDirectoryName|String||
|targetDirectoryName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationRule",
  "editable": true,
  "id": "String (identifier)",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.stringKeyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "name": "String",
  "objectMappings": [
    {
      "@odata.type": "microsoft.graph.objectMapping",
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
            "parameters": [
              {
                "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
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
          "@odata.type": "microsoft.graph.metadataEntry"
        }
      ],
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
  ],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}
```

