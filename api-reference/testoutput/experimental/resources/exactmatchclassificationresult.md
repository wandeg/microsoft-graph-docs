---
title: "exactMatchClassificationResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# exactMatchClassificationResult resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|[detectedSensitiveContent](../resources/detectedSensitiveContent.md) collection||
|errors|[classificationError](../resources/classificationError.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exactMatchClassificationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchClassificationResult",
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
  ],
  "errors": [
    {
      "@odata.type": "microsoft.graph.classificationError",
      "code": "String",
      "message": "String",
      "target": "String",
      "innerError": {
        "@odata.type": "microsoft.graph.classificationInnerError",
        "errorDateTime": "String (timestamp)",
        "clientRequestId": "String",
        "activityId": "String"
      },
      "details": [
        {
          "@odata.type": "microsoft.graph.classifcationErrorBase"
        }
      ]
    }
  ]
}
```

