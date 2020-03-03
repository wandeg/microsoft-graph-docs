---
title: "search resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# search resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get search](../api/search-get.md)|[search](../resources/search.md)|Read properties and relationships of the [search](../resources/search.md) object.|
|[Update search](../api/search-update.md)|[search](../resources/search.md)|Update the properties of a [search](../resources/search.md) object.|
|[query](../api/search-query.md)|[searchResponse](../resources/searchResponse.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search",
  "id": "String (identifier)"
}
```

