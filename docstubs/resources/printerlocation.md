---
title: "printerLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerLocation resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|altitudeInMeters|Int32||
|building|String||
|city|String||
|countryOrRegion|String||
|floorDescription|String||
|floorNumber|Int32||
|latitude|Single||
|longitude|Single||
|organization|String collection||
|postalCode|String||
|roomDescription|String||
|roomNumber|Int32||
|site|String||
|stateOrProvince|String||
|streetAddress|String||
|subdivision|String collection||
|subunit|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Single",
  "longitude": "Single",
  "altitudeInMeters": 1024,
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floorNumber": 1024,
  "floorDescription": "String",
  "roomNumber": 1024,
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

