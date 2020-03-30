---
title: "LIFieldOfStudyArray resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIFieldOfStudyArray resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|fieldsOfStudy|[LIFieldOfStudy](../resources/lifieldofstudy.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIFieldOfStudyArray"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIFieldOfStudyArray",
  "fieldsOfStudy": [
    {
      "@odata.type": "microsoft.graph.LIFieldOfStudy",
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

