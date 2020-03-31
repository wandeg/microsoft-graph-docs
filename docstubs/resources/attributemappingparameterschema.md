---
title: "attributeMappingParameterSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attributeMappingParameterSchema resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowMultipleOccurrences|Boolean||
|name|String||
|required|Boolean||
|type|Enumeration| Possible values are: `DateTime`, `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMappingParameterSchema",
  "allowMultipleOccurrences": true,
  "name": "String",
  "required": true,
  "type": "String"
}
```

