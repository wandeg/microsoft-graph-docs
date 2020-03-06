---
title: "extendedPlacePropertiesModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# extendedPlacePropertiesModel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|businessUrl|String||
|formattedAddress|String||
|menuUrl|String||
|openingHoursSpecifications|[openingHoursSpecification](../resources/openinghoursspecification.md) collection||
|priceRange|String||
|timeZone|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedPlacePropertiesModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedPlacePropertiesModel",
  "priceRange": "String",
  "menuUrl": "String",
  "businessUrl": "String",
  "formattedAddress": "String",
  "openingHoursSpecifications": [
    {
      "@odata.type": "microsoft.graph.openingHoursSpecification",
      "dayOfWeek": "String",
      "opens": "String",
      "closes": "String"
    }
  ],
  "timeZone": "String"
}
```

