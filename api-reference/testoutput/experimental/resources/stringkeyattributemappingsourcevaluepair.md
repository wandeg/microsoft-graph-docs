---
title: "stringKeyAttributeMappingSourceValuePair resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# stringKeyAttributeMappingSourceValuePair resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String||
|value|[attributeMappingSource](../resources/attributemappingsource.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.stringKeyAttributeMappingSourceValuePair",
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.attributeMappingSource",
    "expression": "String",
    "name": "String",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
      }
    ],
    "type": "String"
  }
}
```

