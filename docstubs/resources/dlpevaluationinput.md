---
title: "dlpEvaluationInput resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dlpEvaluationInput resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessScope|Enumeration| Possible values are: `inOrganization`, `notInOrganization`.|
|currentLabel|[currentLabel](../resources/currentlabel.md)||
|discoveredSensitiveTypes|[discoveredSensitiveType](../resources/discoveredsensitivetype.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dlpEvaluationInput"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dlpEvaluationInput",
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
}
```

