---
title: "expressionEvaluationDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# expressionEvaluationDetails resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|expression|String||
|expressionEvaluationDetails|[expressionEvaluationDetails](../resources/expressionEvaluationDetails.md) collection||
|expressionResult|Boolean||
|propertyToEvaluate|[propertyToEvaluate](../resources/propertyToEvaluate.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expressionEvaluationDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expressionEvaluationDetails",
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
  ],
  "propertyToEvaluate": {
    "@odata.type": "microsoft.graph.propertyToEvaluate"
  }
}
```

