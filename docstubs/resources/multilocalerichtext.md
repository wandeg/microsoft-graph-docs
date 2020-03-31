---
title: "MultiLocaleRichText resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# MultiLocaleRichText resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|localized|[RichTextMapElement](../resources/richtextmapelement.md) collection||
|preferredLocale|[Locale](../resources/locale.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.MultiLocaleRichText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.MultiLocaleRichText",
  "localized": [
    {
      "@odata.type": "microsoft.graph.RichTextMapElement",
      "key": "String",
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
                "name": "String",
                "value": "String"
              }
            ]
          }
        ]
      }
    }
  ],
  "preferredLocale": {
    "@odata.type": "microsoft.graph.Locale",
    "language": "String",
    "country": "String",
    "variant": "String"
  }
}
```

