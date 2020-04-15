---
title: "signInLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signInLocation resource type


Namespace: Microsoft.AAD.Reporting



## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String||
|countryOrRegion|String||
|geoCoordinates|[geoCoordinates](../resources/microsoft.aad.reporting-geocoordinates.md)||
|state|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AAD.Reporting.signInLocation"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.signInLocation",
  "city": "String",
  "state": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {
    "@odata.type": "Microsoft.AAD.Reporting.geoCoordinates",
    "altitude": "Double",
    "latitude": "Double",
    "longitude": "Double"
  }
}
```

