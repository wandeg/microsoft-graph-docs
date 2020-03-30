---
title: "SearchMatch resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SearchMatch resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|matchInfo|[LIQueryTermMatchInfo](../resources/liquerytermmatchinfo.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SearchMatch"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SearchMatch",
  "id": "String (identifier)",
  "matchInfo": [
    {
      "@odata.type": "microsoft.graph.LIQueryTermMatchInfo",
      "fieldName": "String"
    }
  ]
}
```

