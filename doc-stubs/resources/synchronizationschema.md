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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[functions](../api/synchronizationschema-functions.md)|[attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) collection|**TODO: Add Description**|
|[filterOperators](../api/synchronizationschema-filteroperators.md)|[filterOperatorSchema](../resources/filteroperatorschema.md) collection|**TODO: Add Description**|
|[parseExpression](../api/synchronizationschema-parseexpression.md)|[parseExpressionResponse](../resources/parseexpressionresponse.md)|**TODO: Add Description**|
|[List directories](../api/synchronizationschema-list-directories.md)|[directoryDefinition](../resources/directorydefinition.md) collection|Get the directoryDefinitions from the directories navigation property.|
|[Create directories](../api/synchronizationschema-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Create a new directories object.|
|[Delete directories](../api/synchronizationschema-delete-directories.md)|None|Delete a [directoryDefinition](../resources/directorydefinition.md) object.|
|[Update directories](../api/synchronizationschema-update-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Update the properties of a directories object.|
|[Get directoryDefinition](../api/directorydefinition-get.md)|[directoryDefinition](../resources/directorydefinition.md)|Read the properties and relationships of a [directoryDefinition](../resources/directorydefinition.md) object.|
|[List schema](../api/synchronizationjob-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchemas from the schema navigation property.|
|[Create schema](../api/synchronizationjob-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new schema object.|

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
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```

