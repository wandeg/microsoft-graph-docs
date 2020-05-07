---
title: "unaryManagementConditionExpression resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unaryManagementConditionExpression resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|operand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|**TODO: Add Description**|
|operator|unaryManagementConditionExpressionOperatorType|**TODO: Add Description**. Possible values are: `not`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```

