---
title: "attributeMappingSource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attributeMappingSource resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|expression|String||
|name|String||
|parameters|[stringKeyAttributeMappingSourceValuePair](../resources/stringkeyattributemappingsourcevaluepair.md) collection||
|type|Enumeration|. Possible values are: `Attribute`, `Constant`, `Function`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attributeMappingSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMappingSource",
  "expression": "String",
  "name": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
      "key": "String",
      "value": {
        "@odata.type": "microsoft.graph.attributeMappingSource",
        "type": "String"
      }
    }
  ],
  "type": "String"
}
```

