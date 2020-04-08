---
title: "LIOrganization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIOrganization resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|industries|[LIIndustry](../resources/liindustry.md) collection||
|locations|[LIOrganizationLocationInfo](../resources/liorganizationlocationinfo.md) collection||
|logoV2|String||
|name|[MultiLocaleString](../resources/multilocalestring.md)||
|website|[MultiLocaleUrl](../resources/multilocaleurl.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIOrganization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIOrganization",
  "id": "String (identifier)",
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
  "logoV2": "String",
  "website": {
    "@odata.type": "microsoft.graph.MultiLocaleUrl",
    "localized": [
      {
        "@odata.type": "microsoft.graph.UrlMapElement"
      }
    ]
  },
  "locations": [
    {
      "@odata.type": "microsoft.graph.LIOrganizationLocationInfo",
      "address": {
        "@odata.type": "microsoft.graph.Address",
        "line1": "String",
        "line2": "String",
        "line3": "String",
        "line4": "String",
        "city": "String",
        "geographicAreaType": "String",
        "geographicArea": "String",
        "postalCode": "String"
      },
      "locationType": "String",
      "standardizedLocation": {
        "@odata.type": "microsoft.graph.LILocation",
        "id": "String",
        "name": "String"
      }
    }
  ],
  "industries": [
    {
      "@odata.type": "microsoft.graph.LIIndustry"
    }
  ]
}
```

