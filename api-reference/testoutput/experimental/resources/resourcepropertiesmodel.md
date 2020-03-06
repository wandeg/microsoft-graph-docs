---
title: "resourcePropertiesModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# resourcePropertiesModel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|bookingType|Enumeration|. Possible values are: `unknown`, `standard`, `reserved`.|
|building|String||
|capacity|Int32||
|floor|String||
|isManaged|Boolean||
|label|String||
|name|String||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourcePropertiesModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourcePropertiesModel",
  "name": "String",
  "label": "String",
  "type": "String",
  "capacity": 1024,
  "isManaged": true,
  "bookingType": "String",
  "building": "String",
  "floor": "String"
}
```

