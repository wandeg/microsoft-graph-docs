---
title: "scoredEmailAddress resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# scoredEmailAddress resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String|**TODO: Add Description**|
|itemId|String|**TODO: Add Description**|
|relevanceScore|Double|**TODO: Add Description**|
|selectionLikelihood|selectionLikelihoodInfo|**TODO: Add Description**. Possible values are: `notSpecified`, `high`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scoredEmailAddress",
  "address": "String",
  "relevanceScore": "Double",
  "selectionLikelihood": "String",
  "itemId": "String"
}
```

