---
title: "place resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# place resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List places](../api/place-list.md)|[place](../resources/place.md) collection|List properties and relationships of the [place](../resources/place.md) objects.|
|[Get place](../api/place-get.md)|[place](../resources/place.md)|Read properties and relationships of the [place](../resources/place.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)||
|displayName|String||
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|phone|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.place",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.place",
  "id": "String (identifier)",
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

