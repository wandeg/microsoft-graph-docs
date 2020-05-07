---
title: "searchHit resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# searchHit resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|_id|String|**TODO: Add Description**|
|_score|Int32|**TODO: Add Description**|
|_sortField|String|**TODO: Add Description**|
|_source|[entity](../resources/entity.md)|**TODO: Add Description**|
|_summary|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchHit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchHit",
  "_id": "String",
  "_score": "Integer",
  "_sortField": "String",
  "_summary": "String",
  "_source": {
    "@odata.type": "#microsoft.graph.entity",
    "id": "String (identifier)"
  }
}
```

