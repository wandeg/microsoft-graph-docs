---
title: "MultiLocaleString resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# MultiLocaleString resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|localized|[StringMapElement](../resources/stringmapelement.md) collection||
|preferredLocale|[Locale](../resources/locale.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.MultiLocaleString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.MultiLocaleString",
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
```

