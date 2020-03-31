---
title: "LIMemberEducation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberEducation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|activities|[MultiLocaleString](../resources/multilocalestring.md)||
|degreeName|[MultiLocaleString](../resources/multilocalestring.md)||
|endMonthYear|[Date](../resources/date.md)||
|fieldsOfStudy|[LIMemberFieldOfStudy](../resources/limemberfieldofstudy.md) collection||
|fieldsOfStudyV2|[LIFieldOfStudy](../resources/lifieldofstudy.md) collection||
|notes|[MultiLocaleRichText](../resources/multilocalerichtext.md)||
|school|[LIOrganization](../resources/liorganization.md)||
|startMonthYear|[Date](../resources/date.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberEducation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberEducation",
  "degreeName": {
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
  "activities": {
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
  "notes": {
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
  "school": {
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
  "fieldsOfStudy": [
    {
      "@odata.type": "microsoft.graph.LIMemberFieldOfStudy",
      "fieldOfStudyName": {
        "@odata.type": "microsoft.graph.MultiLocaleString"
      }
    }
  ],
  "fieldsOfStudyV2": [
    {
      "@odata.type": "microsoft.graph.LIFieldOfStudy"
    }
  ]
}
```

