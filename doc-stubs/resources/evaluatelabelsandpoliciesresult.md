---
title: "evaluateLabelsAndPoliciesResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# evaluateLabelsAndPoliciesResult resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classificationResult|[detectedSensitiveContentWrapper](../resources/detectedsensitivecontentwrapper.md)|**TODO: Add Description**|
|dataLossPreventionPoliciesResult|[dlpPoliciesJobResult](../resources/dlppoliciesjobresult.md)|**TODO: Add Description**|
|sensitivityLabelsResult|[evaluateLabelJobResultGroup](../resources/evaluatelabeljobresultgroup.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesResult",
  "sensitivityLabelsResult": {
    "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup"
  },
  "dataLossPreventionPoliciesResult": {
    "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
  },
  "classificationResult": {
    "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper"
  }
}
```

