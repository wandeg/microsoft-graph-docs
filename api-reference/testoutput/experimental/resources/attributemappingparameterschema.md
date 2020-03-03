---
title: "attributeMappingParameterSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# attributeMappingParameterSchema resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowMultipleOccurrences|Boolean||
|name|String||
|required|Boolean||
|type|Enumeration|. Possible values are: `DateTime`, `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## Relationships
None

## JSON Representation
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

