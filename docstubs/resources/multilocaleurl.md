---
title: "MultiLocaleUrl resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# MultiLocaleUrl resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|localized|[UrlMapElement](../resources/urlmapelement.md) collection||
|preferredLocale|[Locale](../resources/locale.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.MultiLocaleUrl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.MultiLocaleUrl",
  "localized": [
    {
      "@odata.type": "microsoft.graph.UrlMapElement",
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
```

