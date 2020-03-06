---
title: "binaryManagementConditionExpression resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# binaryManagementConditionExpression resource type


Namespace: microsoft.graph




Inherits from [managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|firstOperand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|The first operand of the binary operation.|
|operator|Enumeration|The operator used in the evaluation of the binary operation. Possible values are: `or`, `and`.|
|secondOperand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|The second operand of the binary operation.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

