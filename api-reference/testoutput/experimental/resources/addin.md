---
title: "addIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# addIn resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|Guid||
|properties|[keyValue](../resources/keyValue.md) collection||
|type|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addIn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addIn",
  "id": "String (identifier)",
  "type": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ]
}
```

