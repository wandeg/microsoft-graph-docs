---
title: "LIMemberOrganization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberOrganization resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|
|name|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|position|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|startMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberOrganization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberOrganization",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "position": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "startMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  },
  "endMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  }
}
```

