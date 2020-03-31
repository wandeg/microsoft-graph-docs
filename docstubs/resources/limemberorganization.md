---
title: "LIMemberOrganization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberOrganization resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|endMonthYear|[Date](../resources/date.md)||
|name|[MultiLocaleString](../resources/multilocalestring.md)||
|position|[MultiLocaleString](../resources/multilocalestring.md)||
|startMonthYear|[Date](../resources/date.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberOrganization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberOrganization",
  "name": {
    "@odata.type": "microsoft.graph.MultiLocaleString",
    "localized": [
      {
        "@odata.type": "microsoft.graph.StringMapElement",
        "key": "String",
        "value": "String"
      }
    ],
    "preferredLocale": {
      "@odata.type": "microsoft.graph.Locale",
      "language": "String",
      "country": "String",
      "variant": "String"
    }
  },
  "position": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "startMonthYear": {
    "@odata.type": "microsoft.graph.Date",
    "day": 1024,
    "month": 1024,
    "year": 1024
  },
  "endMonthYear": {
    "@odata.type": "microsoft.graph.Date"
  }
}
```

