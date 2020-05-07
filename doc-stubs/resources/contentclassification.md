---
title: "contentClassification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# contentClassification resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|confidence|Int32|**TODO: Add Description**|
|matches|[matchLocation](../resources/matchlocation.md) collection|**TODO: Add Description**|
|sensitiveTypeId|String|**TODO: Add Description**|
|uniqueCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentClassification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentClassification",
  "sensitiveTypeId": "String",
  "uniqueCount": "Integer",
  "confidence": "Integer",
  "matches": [
    {
      "@odata.type": "microsoft.graph.matchLocation"
    }
  ]
}
```

