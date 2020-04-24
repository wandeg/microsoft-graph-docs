---
title: "extendedPlacePropertiesModel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# extendedPlacePropertiesModel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|businessUrl|String|**TODO: Add Description**|
|formattedAddress|String|**TODO: Add Description**|
|menuUrl|String|**TODO: Add Description**|
|openingHoursSpecifications|[openingHoursSpecification](../resources/openinghoursspecification.md) collection|**TODO: Add Description**|
|priceRange|String|**TODO: Add Description**|
|timeZone|String|**TODO: Add Description**|

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

