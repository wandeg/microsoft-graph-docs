---
title: "companyDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# companyDetail resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)||
|department|String||
|displayName|String||
|officeLocation|String||
|pronunciation|String||
|webUrl|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyDetail",
  "displayName": "String",
  "pronunciation": "String",
  "department": "String",
  "officeLocation": "String",
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
  "webUrl": "String"
}
```

