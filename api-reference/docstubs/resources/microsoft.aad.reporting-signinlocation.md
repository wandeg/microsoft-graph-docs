---
title: "signInLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "Microsoft.AAD.Reporting.geoCoordinates"
  }
}
```

