---
title: "dlpEvaluatePoliciesRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# dlpEvaluatePoliciesRequest resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|evaluationInput|[dlpEvaluationInput](../resources/dlpEvaluationInput.md)||
|notificationInfo|[dlpNotification](../resources/dlpNotification.md)||
|target|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dlpEvaluatePoliciesRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesRequest",
  "target": "String",
  "evaluationInput": {
    "@odata.type": "microsoft.graph.dlpEvaluationInput",
    "discoveredSensitiveTypes": [
      {
        "@odata.type": "microsoft.graph.discoveredSensitiveType",
        "id": "Guid",
        "count": 1024,
        "confidence": 1024
      }
    ],
    "currentLabel": {
      "@odata.type": "microsoft.graph.currentLabel",
      "id": "String",
      "applicationMode": "String"
    },
    "accessScope": "String"
  },
  "notificationInfo": {
    "@odata.type": "microsoft.graph.dlpNotification",
    "author": "String"
  }
}
```

