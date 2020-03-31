---
title: "LIMemberHonor resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberHonor resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[MultiLocaleRichText](../resources/multilocalerichtext.md)||
|issueDate|[Date](../resources/date.md)||
|issuer|[MultiLocaleString](../resources/multilocalestring.md)||
|title|[MultiLocaleString](../resources/multilocalestring.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberHonor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberHonor",
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
  "issueDate": {
    "@odata.type": "microsoft.graph.Date",
    "day": 1024,
    "month": 1024,
    "year": 1024
  },
  "issuer": {
    "@odata.type": "microsoft.graph.MultiLocaleString"
  }
}
```

