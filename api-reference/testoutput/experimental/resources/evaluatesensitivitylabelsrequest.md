---
title: "evaluateSensitivityLabelsRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# evaluateSensitivityLabelsRequest resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentLabel|[currentLabel](../resources/currentLabel.md)||
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredSensitiveType.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateSensitivityLabelsRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateSensitivityLabelsRequest",
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
  }
}
```

