---
title: "LIOrganizationLocationInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# LIOrganizationLocationInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[Address](../resources/address.md)||
|locationType|Enumeration| Possible values are: `HEADQUARTERS`, `OTHER`.|
|standardizedLocation|[LILocation](../resources/lilocation.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.LIOrganizationLocationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.LIOrganizationLocationInfo",
  "address": {
    "@odata.type": "microsoft.graph.Address",
    "line1": "String",
    "line2": "String",
    "line3": "String",
    "line4": "String",
    "city": "String",
    "geographicAreaType": "String",
    "geographicArea": "String",
    "postalCode": "String",
    "country": "String"
  },
  "locationType": "String",
  "standardizedLocation": {
    "@odata.type": "microsoft.graph.LILocation",
    "id": "String",
    "name": "String"
  }
}
```

