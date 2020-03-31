---
title: "LIMemberProject resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberProject resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[MultiLocaleRichText](../resources/multilocalerichtext.md)||
|endMonthYear|[Date](../resources/date.md)||
|startMonthYear|[Date](../resources/date.md)||
|title|[MultiLocaleString](../resources/multilocalestring.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberProject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberProject",
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
  }
}
```

