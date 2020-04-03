---
title: "institutionData resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# institutionData resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|location|[physicalAddress](../resources/physicaladdress.md)||
|webUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.institutionData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.institutionData",
  "description": "String",
  "displayName": "String",
  "location": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "String",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryOrRegion": "String",
    "postalCode": "String"
  },
  "webUrl": "String"
}
```

