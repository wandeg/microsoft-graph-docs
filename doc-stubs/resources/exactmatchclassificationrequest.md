---
title: "exactMatchClassificationRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# exactMatchClassificationRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentClassifications|[contentClassification](../resources/contentclassification.md) collection|**TODO: Add Description**|
|sensitiveTypeIds|String collection|**TODO: Add Description**|
|text|String|**TODO: Add Description**|
|timeoutInMs|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "timeoutInMs": "Integer",
  "contentClassifications": [
    {
      "@odata.type": "microsoft.graph.contentClassification"
    }
  ]
}
```

