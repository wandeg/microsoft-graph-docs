---
title: "LIMemberPosition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberPosition resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|company|[LIOrganization](../resources/liorganization.md)||
|description|[MultiLocaleRichText](../resources/multilocalerichtext.md)||
|endMonthYear|[Date](../resources/date.md)||
|locationName|[MultiLocaleString](../resources/multilocalestring.md)||
|startMonthYear|[Date](../resources/date.md)||
|title|[MultiLocaleString](../resources/multilocalestring.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberPosition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberPosition",
  "title": {
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
  "description": {
    "@odata.type": "microsoft.graph.MultiLocaleRichText",
    "localized": [
      {
        "@odata.type": "microsoft.graph.RichTextMapElement",
        "value": {
          "@odata.type": "microsoft.graph.RichText",
          "rawText": "String",
          "rtData": [
            {
              "@odata.type": "microsoft.graph.RTData",
              "type": "String",
              "startIdx": 1024,
              "endIdx": 1024,
              "attribute": [
                {
                  "@odata.type": "microsoft.graph.RTAttribute",
                  "name": "String"
                }
              ]
            }
          ]
        }
      }
    ]
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
  "company": {
    "@odata.type": "microsoft.graph.LIOrganization",
    "id": "String",
    "name": {
      "@odata.type": "microsoft.graph.MultiLocaleString"
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
          "@odata.type": "microsoft.graph.LILocation"
        }
      }
    ],
    "industries": [
      {
        "@odata.type": "microsoft.graph.LIIndustry"
      }
    ]
  },
  "locationName": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  }
}
```

