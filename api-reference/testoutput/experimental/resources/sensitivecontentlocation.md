---
title: "sensitiveContentLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sensitiveContentLocation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|evidences|[sensitiveContentEvidence](../resources/sensitiveContentEvidence.md) collection||
|idMatch|String||
|length|Int32||
|offset|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sensitiveContentLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitiveContentLocation",
  "idMatch": "String",
  "offset": 1024,
  "length": 1024,
  "evidences": [
    {
      "@odata.type": "microsoft.graph.sensitiveContentEvidence",
      "match": "String"
    }
  ]
}
```

