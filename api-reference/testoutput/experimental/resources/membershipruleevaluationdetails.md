---
title: "membershipRuleEvaluationDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# membershipRuleEvaluationDetails resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|membershipRuleEvaluationDetails|[expressionEvaluationDetails](../resources/expressionEvaluationDetails.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membershipRuleEvaluationDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membershipRuleEvaluationDetails",
  "membershipRuleEvaluationDetails": {
    "@odata.type": "microsoft.graph.expressionEvaluationDetails",
    "expressionResult": true,
    "expression": "String",
    "expressionEvaluationDetails": [
      {
        "@odata.type": "microsoft.graph.expressionEvaluationDetails",
        "propertyToEvaluate": {
          "@odata.type": "microsoft.graph.propertyToEvaluate",
          "propertyName": "String",
          "propertyValue": "String"
        }
      }
    ]
  }
}
```

