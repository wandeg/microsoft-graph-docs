---
title: "countryNamedLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# countryNamedLocation resource type




Inherits from [namedLocation](../resources/namedLocation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List countryNamedLocations](../api/countrynamedlocation-list.md)|[countryNamedLocation](../resources/countryNamedLocation.md) collection|List properties and relationships of the [countryNamedLocation](../resources/countrynamedlocation.md) objects.|
|[Get countryNamedLocation](../api/countrynamedlocation-get.md)|[countryNamedLocation](../resources/countryNamedLocation.md)|Read properties and relationships of the [countryNamedLocation](../resources/countrynamedlocation.md) object.|
|[Create countryNamedLocation](../api/countrynamedlocation-create.md)|[countryNamedLocation](../resources/countryNamedLocation.md)|Create a new [countryNamedLocation](../resources/countrynamedlocation.md) object.|
|[Delete countryNamedLocation](../api/countrynamedlocation-delete.md)|None|Deletes a [countryNamedLocation](../resources/countrynamedlocation.md).|
|[Update countryNamedLocation](../api/countrynamedlocation-update.md)|[countryNamedLocation](../resources/countryNamedLocation.md)|Update the properties of a [countryNamedLocation](../resources/countrynamedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|countriesAndRegions|String collection||
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedLocation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|includeUnknownCountriesAndRegions|Boolean||
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": "microsoft.graph.namedLocation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "countriesAndRegions": [
    "String"
  ],
  "includeUnknownCountriesAndRegions": true
}
```

