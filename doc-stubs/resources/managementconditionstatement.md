---
title: "managementConditionStatement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managementConditionStatement resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getManagementConditionStatementExpressionString](../api/managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/managementconditionexpressionstring.md)|**TODO: Add Description**|
|[getManagementConditionStatementsForPlatform](../api/managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|**TODO: Add Description**|
|[List managementConditions](../api/managementconditionstatement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Add managementConditions](../api/managementconditionstatement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Add managementConditions by posting to the managementConditions collection.|
|[Remove managementConditions](../api/managementconditionstatement-delete-managementconditions.md)|None|Remove a [managementCondition](../resources/managementcondition.md) object.|
|[List managementConditionStatements](../api/managementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Add managementConditionStatements](../api/managementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Add managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|devicePlatformType collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|eTag|String|**TODO: Add Description**|
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/managementcondition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```

