---
title: "synchronizationSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationSchema resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List synchronizationSchemas](../api/synchronizationschema-list.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|List properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) objects.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Create synchronizationSchema](../api/synchronizationschema-create.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Delete synchronizationSchema](../api/synchronizationschema-delete.md)|None|Deletes a [synchronizationSchema](../resources/synchronizationschema.md).|
|[Update synchronizationSchema](../api/synchronizationschema-update.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[functions](../api/synchronizationschema-functions.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection||
|[filterOperators](../api/synchronizationschema-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection||
|[parseExpression](../api/synchronizationschema-parseexpression.md)|[parseExpressionResponse](../resources/parseexpressionresponse.md)||
|[List directories](../api/synchronizationschema-list-directories.md)|[directoryDefinition](../resources/directorydefinition.md) collection|Get the directoryDefinitions from the directories navigation property.|
|[Add directories](../api/synchronizationschema-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Add directories by posting to the directories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|provisioningTaskIdentifier|String||
|synchronizationRules|[synchronizationRule](../resources/synchronizationrule.md) collection||
|version|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directories|[directoryDefinition](../resources/directorydefinition.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "provisioningTaskIdentifier": "String",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule",
      "editable": true,
      "id": "String",
      "metadata": [
        {
          "@odata.type": "microsoft.graph.stringKeyStringValuePair"
        }
      ],
      "objectMappings": [
        {
          "@odata.type": "microsoft.graph.objectMapping",
          "attributeMappings": [
            {
              "@odata.type": "microsoft.graph.attributeMapping",
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
  ],
  "version": "String"
}
```

