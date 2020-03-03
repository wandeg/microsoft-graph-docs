---
title: "exactMatchClassificationRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# exactMatchClassificationRequest resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentClassifications|[contentClassification](../resources/contentclassification.md) collection||
|sensitiveTypeIds|String collection||
|text|String||
|timeoutInMs|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exactMatchClassificationRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchClassificationRequest",
  "sensitiveTypeIds": [
    "String"
  ],
  "text": "String",
  "timeoutInMs": 1024,
  "contentClassifications": [
    {
      "@odata.type": "microsoft.graph.contentClassification",
      "sensitiveTypeId": "String",
      "uniqueCount": 1024,
      "confidence": 1024,
      "matches": [
        {
          "@odata.type": "microsoft.graph.matchLocation",
          "length": 1024,
          "offset": 1024
        }
      ]
    }
  ]
}
```

