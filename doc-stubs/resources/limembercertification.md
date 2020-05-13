---
title: "LIMemberCertification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# LIMemberCertification resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authority|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|company|[LIOrganization](../resources/liorganization.md)|**TODO: Add Description**|
|endMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|
|licenseNumber|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|name|[MultiLocaleString](../resources/multilocalestring.md)|**TODO: Add Description**|
|startMonthYear|[Date](../resources/date.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberCertification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberCertification",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "licenseNumber": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "authority": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "startMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  },
  "endMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  },
  "url": "String",
  "company": {
    "@odata.type": "microsoft.graph.LIOrganization"
  }
}
```

