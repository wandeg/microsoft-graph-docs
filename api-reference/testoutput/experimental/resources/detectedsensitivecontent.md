---
title: "detectedSensitiveContent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# detectedSensitiveContent resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|confidence|Int32||
|displayName|String||
|id|Guid||
|matches|[sensitiveContentLocation](../resources/sensitivecontentlocation.md) collection||
|recommendedConfidence|Int32||
|uniqueCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detectedSensitiveContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedSensitiveContent",
  "id": "String (identifier)",
  "displayName": "String",
  "uniqueCount": 1024,
  "confidence": 1024,
  "recommendedConfidence": 1024,
  "matches": [
    {
      "@odata.type": "microsoft.graph.sensitiveContentLocation",
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
  ]
}
```

