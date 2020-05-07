---
title: "binaryManagementConditionExpression resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# binaryManagementConditionExpression resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|firstOperand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|**TODO: Add Description**|
|operator|binaryManagementConditionExpressionOperatorType|**TODO: Add Description**. Possible values are: `or`, `and`.|
|secondOperand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```

