---
title: "managementConditionStatement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managementConditionStatement resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managementConditionStatement](../api/managementconditionstatement-get.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Read properties and relationships of the [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Update managementConditionStatement](../api/managementconditionstatement-update.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Update the properties of a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[getManagementConditionStatementExpressionString](../api/managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/managementconditionexpressionstring.md)||
|[getManagementConditionStatementsForPlatform](../api/managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection||
|[List managementConditions](../api/managementconditionstatement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Create managementConditions](../api/managementconditionstatement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Create managementConditions by posting to the managementConditions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|eTag|String||
|expression|[managementConditionExpression](../resources/managementconditionexpression.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/managementcondition.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

