---
title: "managementConditionStatement resource type"
description: "A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managementConditionStatement resource type

A management condition statement is a group of management conditions that enable/disable device/application configurations when all contained management conditions are met.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managementConditionStatement](../api/managementconditionstatement-get.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Read properties and relationships of the [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[Delete managementConditionStatement](../api/managementconditionstatement-delete.md)|None|Deletes a [managementConditionStatement](../resources/managementconditionstatement.md).|
|[Update managementConditionStatement](../api/managementconditionstatement-update.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Update the properties of a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[getManagementConditionStatementExpressionString](../api/managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/managementConditionExpressionString.md)||
|[getManagementConditionStatementsForPlatform](../api/managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/managementConditionStatement.md) collection||
|[List managementConditions](../api/managementconditionstatement-list-managementconditions.md)|[managementCondition](../resources/managementCondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Create managementConditions](../api/managementconditionstatement-post-managementconditions.md)|[managementCondition](../resources/managementCondition.md)|Create managementConditions by posting to the managementConditions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition statement.
This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.|
|createdDateTime|DateTimeOffset|The time the management condition statement was created. Generated service side.|
|description|String|The admin defined description of the management condition statement.|
|displayName|String|The admin defined name of the management condition statement.|
|eTag|String|ETag of the management condition statement. Updated service side.|
|expression|[managementConditionExpression](../resources/managementConditionExpression.md)|The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.|
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|The time the management condition statement was last modified. Updated service side.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/managementCondition.md) collection|The management conditions associated to the management condition statement.|

## JSON Representation
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

