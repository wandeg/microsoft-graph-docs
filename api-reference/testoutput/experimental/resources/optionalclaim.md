---
title: "optionalClaim resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# optionalClaim resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|additionalProperties|String collection||
|essential|Boolean||
|name|String||
|source|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaim"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.optionalClaim",
  "name": "String",
  "source": "String",
  "essential": true,
  "additionalProperties": [
    "String"
  ]
}
```

