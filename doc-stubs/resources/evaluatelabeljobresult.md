---
title: "evaluateLabelJobResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# evaluateLabelJobResult resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|responsiblePolicy|[responsiblePolicy](../resources/responsiblepolicy.md)|**TODO: Add Description**|
|responsibleSensitiveTypes|[responsibleSensitiveType](../resources/responsiblesensitivetype.md) collection|**TODO: Add Description**|
|sensitivityLabel|[matchingLabel](../resources/matchinglabel.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateLabelJobResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResult",
  "sensitivityLabel": {
    "@odata.type": "microsoft.graph.matchingLabel"
  },
  "responsibleSensitiveTypes": [
    {
      "@odata.type": "microsoft.graph.responsibleSensitiveType"
    }
  ],
  "responsiblePolicy": {
    "@odata.type": "microsoft.graph.responsiblePolicy"
  }
}
```

