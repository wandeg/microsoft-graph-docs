---
title: "searchQuery resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# searchQuery resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|query_string|[searchQueryString](../resources/searchQueryString.md)||

## Relationships
None

## JSON Representation
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

