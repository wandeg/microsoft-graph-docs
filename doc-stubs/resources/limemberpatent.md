---
title: "LIMemberPatent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberPatent resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[MultiLocaleRichText](../resources/multilocalerichtext.md)|**TODO: Add Description**|
|issueDate|[Date](../resources/date.md)|**TODO: Add Description**|
|issuer|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|number|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|pending|Boolean|**TODO: Add Description**|
|title|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberPatent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberPatent",
  "title": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "issuer": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "pending": "Boolean",
  "number": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "url": "String",
  "description": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText"
  },
  "issueDate": {
    "@odata.type": "microsoft.graph.Date"
  }
}
```

