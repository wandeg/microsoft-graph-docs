---
title: "expressionEvaluationDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# expressionEvaluationDetails resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|expression|String||
|expressionEvaluationDetails|[expressionEvaluationDetails](../resources/expressionevaluationdetails.md) collection||
|expressionResult|Boolean||
|propertyToEvaluate|[propertyToEvaluate](../resources/propertytoevaluate.md)||

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

