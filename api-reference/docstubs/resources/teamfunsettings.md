---
title: "teamFunSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# teamFunSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowCustomMemes|Boolean|**TODO: Add Description**|
|allowGiphy|Boolean|**TODO: Add Description**|
|allowStickersAndMemes|Boolean|**TODO: Add Description**|
|giphyContentRating|giphyRatingType|**TODO: Add Description**. Possible values are: `moderate`, `strict`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamFunSettings",
  "allowGiphy": true,
  "giphyContentRating": "String",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

