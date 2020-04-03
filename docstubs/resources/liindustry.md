---
title: "LIIndustry resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIIndustry resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String||
|name|[MultiLocaleString](../resources/multilocalestring.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIIndustry"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIIndustry",
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
  }
}
```

