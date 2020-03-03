---
title: "evaluateDynamicMembershipResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# evaluateDynamicMembershipResult resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|membershipRule|String||
|membershipRuleEvaluationDetails|[expressionEvaluationDetails](../resources/expressionEvaluationDetails.md)||
|membershipRuleEvaluationResult|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateDynamicMembershipResult",
  "membershipRule": "String",
  "membershipRuleEvaluationResult": true,
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

