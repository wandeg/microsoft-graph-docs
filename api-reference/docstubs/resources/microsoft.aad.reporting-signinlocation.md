---
title: "signInLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# signInLocation resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String|**TODO: Add Description**|
|countryOrRegion|String|**TODO: Add Description**|
|geoCoordinates|[geoCoordinates](../resources/microsoft.aad.reporting-geocoordinates.md)|**TODO: Add Description**|
|state|String|**TODO: Add Description**|

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

