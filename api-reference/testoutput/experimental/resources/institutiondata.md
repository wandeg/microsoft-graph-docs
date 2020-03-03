---
title: "institutionData resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# institutionData resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|location|[physicalAddress](../resources/physicalAddress.md)||
|webUrl|String||

## Relationships
None

## JSON Representation
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

