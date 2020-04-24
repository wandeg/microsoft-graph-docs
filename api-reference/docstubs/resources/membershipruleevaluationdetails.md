---
title: "membershipRuleEvaluationDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# membershipRuleEvaluationDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|membershipRuleEvaluationDetails|[expressionEvaluationDetails](../resources/expressionevaluationdetails.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

