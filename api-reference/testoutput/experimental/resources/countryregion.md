---
title: "countryRegion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# countryRegion resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get countryRegion](../api/countryregion-get.md)|[countryRegion](../resources/countryregion.md)|Read properties and relationships of the [countryRegion](../resources/countryregion.md) object.|
|[Update countryRegion](../api/countryregion-update.md)|[countryRegion](../resources/countryregion.md)|Update the properties of a [countryRegion](../resources/countryregion.md) object.|
|[List countriesRegions](../api/company-list-countriesregions.md)|[countryRegion](../resources/countryregion.md) collection|Get the countryRegions from the countriesRegions navigation property.|
|[Add countriesRegions](../api/company-post-countriesregions.md)|[countryRegion](../resources/countryregion.md)|Add countriesRegions by posting to the countriesRegions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addressFormat|String||
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.countryRegion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.countryRegion",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "addressFormat": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

