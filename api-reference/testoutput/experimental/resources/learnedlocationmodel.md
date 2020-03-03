---
title: "learnedLocationModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# learnedLocationModel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)||
|coordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.learnedLocationModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.learnedLocationModel",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "String",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryOrRegion": "String",
    "postalCode": "String"
  },
  "coordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double",
    "accuracy": "Double",
    "altitudeAccuracy": "Double"
  }
}
```

