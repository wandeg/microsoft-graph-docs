---
title: "Address resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# Address resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|city|String||
|country|String||
|geographicArea|String||
|geographicAreaType|Enumeration| Possible values are: `PROVINCE`, `STATE`.|
|line1|String||
|line2|String||
|line3|String||
|line4|String||
|postalCode|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Address"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Address",
  "line1": "String",
  "line2": "String",
  "line3": "String",
  "line4": "String",
  "city": "String",
  "geographicAreaType": "String",
  "geographicArea": "String",
  "postalCode": "String",
  "country": "String"
}
```

