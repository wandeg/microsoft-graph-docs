---
title: "synchronizationRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationRule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|editable|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|metadata|[stringKeyStringValuePair](../resources/stringkeystringvaluepair.md) collection|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|objectMappings|[objectMapping](../resources/objectmapping.md) collection|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|sourceDirectoryName|String|**TODO: Add Description**|
|targetDirectoryName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

