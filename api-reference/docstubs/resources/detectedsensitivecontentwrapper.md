---
title: "detectedSensitiveContentWrapper resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# detectedSensitiveContentWrapper resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|[detectedSensitiveContent](../resources/detectedsensitivecontent.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

