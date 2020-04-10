---
title: "addHeader resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# addHeader resource type


Namespace: microsoft.graph




Inherits from [markContent](../resources/markcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alignment|Enumeration| Possible values are: `left`, `right`, `center`.|
|fontColor|String| Inherited from [markContent](../resources/markcontent.md)|
|fontSize|Int64| Inherited from [markContent](../resources/markcontent.md)|
|margin|Int32||
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|
|text|String| Inherited from [markContent](../resources/markcontent.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addHeader"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addHeader",
  "name": "String",
  "fontSize": 1024,
  "text": "String",
  "fontColor": "String",
  "margin": 1024,
  "alignment": "String"
}
```

