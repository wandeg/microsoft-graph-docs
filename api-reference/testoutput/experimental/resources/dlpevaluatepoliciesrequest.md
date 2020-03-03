---
title: "dlpEvaluatePoliciesRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dlpEvaluatePoliciesRequest resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|evaluationInput|[dlpEvaluationInput](../resources/dlpevaluationinput.md)||
|notificationInfo|[dlpNotification](../resources/dlpnotification.md)||
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

