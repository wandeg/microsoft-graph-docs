---
title: "positionDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# positionDetail resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|company|[companyDetail](../resources/companydetail.md)||
|description|String||
|endMonthYear|Date||
|jobTitle|String||
|role|String||
|startMonthYear|Date||
|summary|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.positionDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.positionDetail",
  "company": {
    "@odata.type": "microsoft.graph.companyDetail",
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
  },
  "description": "String",
  "endMonthYear": "Date",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "Date",
  "summary": "String"
}
```

