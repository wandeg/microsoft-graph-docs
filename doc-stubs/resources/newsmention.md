---
title: "NewsMention resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# NewsMention resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdOn|[Date](../resources/date.md)|**TODO: Add Description**|
|snippet|String|**TODO: Add Description**|
|thumbnail|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.NewsMention"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.NewsMention",
  "title": "String",
  "snippet": "String",
  "url": "String",
  "createdOn": {
    "@odata.type": "microsoft.graph.Date"
  },
  "thumbnail": "String"
}
```

