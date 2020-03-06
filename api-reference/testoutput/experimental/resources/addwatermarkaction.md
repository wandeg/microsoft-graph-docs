---
title: "addWatermarkAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# addWatermarkAction resource type


Namespace: microsoft.graph




Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

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

## JSON representation
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

