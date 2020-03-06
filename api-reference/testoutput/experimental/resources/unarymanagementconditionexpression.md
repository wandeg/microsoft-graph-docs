---
title: "unaryManagementConditionExpression resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unaryManagementConditionExpression resource type


Namespace: microsoft.graph




Inherits from [managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|operand|[managementConditionExpressionModel](../resources/managementconditionexpressionmodel.md)|The operand of the unary operation.|
|operator|Enumeration|The operator used in the evaluation of the unary operation. Possible values are: `not`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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

