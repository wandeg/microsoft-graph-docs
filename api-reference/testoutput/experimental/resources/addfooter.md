---
title: "addFooter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# addFooter resource type




Inherits from [markContent](../resources/markContent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alignment|Enumeration|. Possible values are: `left`, `right`, `center`.|
|fontColor|String| Inherited from [markContent](../resources/markContent.md)|
|fontSize|Int64| Inherited from [markContent](../resources/markContent.md)|
|margin|Int32||
|name|String| Inherited from [labelActionBase](../resources/labelActionBase.md)|
|text|String| Inherited from [markContent](../resources/markContent.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addFooter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addFooter",
  "name": "String",
  "fontSize": 1024,
  "text": "String",
  "fontColor": "String",
  "margin": 1024,
  "alignment": "String"
}
```

