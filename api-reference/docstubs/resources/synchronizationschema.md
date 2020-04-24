---
title: "synchronizationSchema resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationSchema resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Update synchronizationSchema](../api/synchronizationschema-update.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[functions](../api/synchronizationschema-functions.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection|**TODO: Add Description**|
|[filterOperators](../api/synchronizationschema-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection|**TODO: Add Description**|
|[parseExpression](../api/synchronizationschema-parseexpression.md)|[parseExpressionResponse](../resources/parseexpressionresponse.md)|**TODO: Add Description**|
|[List directories](../api/synchronizationschema-list-directories.md)|[directoryDefinition](../resources/directorydefinition.md) collection|Get the directoryDefinitions from the directories navigation property.|
|[Create directories](../api/synchronizationschema-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Create a new directories object.|
|[Delete directories](../api/synchronizationschema-delete-directories.md)|None|Delete a [directoryDefinition](../resources/directorydefinition.md) object.|
|[Update directories](../api/synchronizationschema-update-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Update the properties of a directories object.|
|[Get directoryDefinition](../api/directorydefinition-get.md)|[directoryDefinition](../resources/directorydefinition.md)|Read the properties and relationships of a [directoryDefinition](../resources/directorydefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|provisioningTaskIdentifier|String|**TODO: Add Description**|
|synchronizationRules|[synchronizationRule](../resources/synchronizationrule.md) collection|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directories|[directoryDefinition](../resources/directorydefinition.md) collection|**TODO: Add Description**|

## JSON representation
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

