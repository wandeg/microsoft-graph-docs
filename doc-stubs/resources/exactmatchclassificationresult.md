---
title: "exactMatchClassificationResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# exactMatchClassificationResult resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classification|[exactMatchDetectedSensitiveContent](../resources/exactmatchdetectedsensitivecontent.md) collection|**TODO: Add Description**|
|errors|[classificationError](../resources/classificationerror.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.exactMatchDetectedSensitiveContent"
    }
  ],
  "errors": [
    {
      "@odata.type": "microsoft.graph.classificationError"
    }
  ]
}
```

