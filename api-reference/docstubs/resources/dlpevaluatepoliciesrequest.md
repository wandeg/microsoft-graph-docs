---
title: "dlpEvaluatePoliciesRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# dlpEvaluatePoliciesRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|evaluationInput|[dlpEvaluationInput](../resources/dlpevaluationinput.md)|**TODO: Add Description**|
|notificationInfo|[dlpNotification](../resources/dlpnotification.md)|**TODO: Add Description**|
|target|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

