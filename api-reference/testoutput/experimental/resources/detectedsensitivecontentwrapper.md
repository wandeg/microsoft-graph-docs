---
title: "detectedSensitiveContentWrapper resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# detectedSensitiveContentWrapper resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|[detectedSensitiveContent](../resources/detectedsensitivecontent.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedSensitiveContentWrapper",
  "classification": [
    {
      "@odata.type": "microsoft.graph.detectedSensitiveContent",
      "id": "Guid",
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
  ]
}
```

