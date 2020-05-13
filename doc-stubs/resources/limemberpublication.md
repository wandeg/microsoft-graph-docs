---
title: "LIMemberPublication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberPublication resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|date|[Date](../resources/date.md)|**TODO: Add Description**|
|description|[MultiLocaleRichText](../resources/multilocalerichtext.md)|**TODO: Add Description**|
|name|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|publisher|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberPublication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberPublication",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "description": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText"
  },
  "date": {
    "@odata.type": "microsoft.graph.Date"
  },
  "publisher": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "url": "String"
}
```

