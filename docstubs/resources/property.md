---
title: "property resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# property resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isQueryable|Boolean||
|isRetrievable|Boolean||
|isSearchable|Boolean||
|name|String||
|type|Enumeration| Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.property"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.property",
  "name": "String",
  "type": "String",
  "isSearchable": true,
  "isRetrievable": true,
  "isQueryable": true
}
```

