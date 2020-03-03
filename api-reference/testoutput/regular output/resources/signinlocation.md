---
title: "signInLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# signInLocation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String||
|countryOrRegion|String||
|geoCoordinates|[geoCoordinates](../resources/geoCoordinates.md)||
|state|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signInLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signInLocation",
  "city": "String",
  "state": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  }
}
```

