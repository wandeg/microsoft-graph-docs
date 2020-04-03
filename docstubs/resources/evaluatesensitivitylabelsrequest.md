---
title: "evaluateSensitivityLabelsRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# evaluateSensitivityLabelsRequest resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|currentLabel|[currentLabel](../resources/currentlabel.md)||
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredsensitivetype.md) collection||

## Relationships
None

## JSON representation
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

