---
title: "LITitleArray resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LITitleArray resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|titles|[LITitle](../resources/lititle.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LITitleArray"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LITitleArray",
  "titles": [
    {
      "@odata.type": "microsoft.graph.LITitle",
      "id": "String",
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
      }
    }
  ]
}
```

