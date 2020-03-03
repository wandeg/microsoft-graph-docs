---
title: "addWatermarkAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# addWatermarkAction resource type




Inherits from [informationProtectionAction](../resources/informationProtectionAction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fontColor|String||
|fontName|String||
|fontSize|Int32||
|layout|Enumeration|. Possible values are: `horizontal`, `diagonal`.|
|text|String||
|uiElementName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addWatermarkAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addWatermarkAction",
  "uiElementName": "String",
  "layout": "String",
  "text": "String",
  "fontName": "String",
  "fontSize": 1024,
  "fontColor": "String"
}
```

