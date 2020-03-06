---
title: "searchQuery resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# searchQuery resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|query_string|[searchQueryString](../resources/searchquerystring.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchQuery"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchQuery",
  "query_string": {
    "@odata.type": "microsoft.graph.searchQueryString",
    "query": "String"
  }
}
```

