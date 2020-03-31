---
title: "LIMemberLanguage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIMemberLanguage resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|[MultiLocaleString](../resources/multilocalestring.md)||
|proficiency|Enumeration| Possible values are: `ELEMENTARY`, `LIMITED_WORKING`, `PROFESSIONAL_WORKING`, `FULL_PROFESSIONAL`, `NATIVE_OR_BILINGUAL`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIMemberLanguage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIMemberLanguage",
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
  "proficiency": "String"
}
```

