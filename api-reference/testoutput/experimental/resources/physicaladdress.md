---
title: "physicalAddress resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# physicalAddress resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String||
|countryOrRegion|String||
|postalCode|String||
|postOfficeBox|String||
|state|String||
|street|String||
|type|Enumeration|. Possible values are: `unknown`, `home`, `business`, `other`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.physicalAddress"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.physicalAddress",
  "type": "String",
  "postOfficeBox": "String",
  "street": "String",
  "city": "String",
  "state": "String",
  "countryOrRegion": "String",
  "postalCode": "String"
}
```

