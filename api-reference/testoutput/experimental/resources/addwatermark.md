---
title: "addWatermark resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# addWatermark resource type


Namespace: microsoft.graph




Inherits from [markContent](../resources/markcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fontColor|String| Inherited from [markContent](../resources/markcontent.md)|
|fontSize|Int64| Inherited from [markContent](../resources/markcontent.md)|
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|
|orientation|Enumeration|. Possible values are: `horizontal`, `diagonal`.|
|text|String| Inherited from [markContent](../resources/markcontent.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addWatermark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addWatermark",
  "name": "String",
  "fontSize": 1024,
  "text": "String",
  "fontColor": "String",
  "orientation": "String"
}
```

