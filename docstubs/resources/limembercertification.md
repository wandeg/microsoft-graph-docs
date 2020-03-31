---
title: "LIMemberCertification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberCertification resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|authority|[MultiLocaleString](../resources/multilocalestring.md)||
|company|[LIOrganization](../resources/liorganization.md)||
|endMonthYear|[Date](../resources/date.md)||
|licenseNumber|[MultiLocaleString](../resources/multilocalestring.md)||
|name|[MultiLocaleString](../resources/multilocalestring.md)||
|startMonthYear|[Date](../resources/date.md)||
|url|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberCertification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberCertification",
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
  "licenseNumber": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  },
  "authority": {
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
  },
  "url": "String",
  "company": {
    "@odata.type": "microsoft.graph.LIOrganization",
    "id": "String",
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
}
```

