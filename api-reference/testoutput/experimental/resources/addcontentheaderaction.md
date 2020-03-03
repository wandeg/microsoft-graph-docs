---
title: "addContentHeaderAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# addContentHeaderAction resource type


Namespace: microsoft.graph




Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alignment|Enumeration|. Possible values are: `left`, `right`, `center`.|
|fontColor|String||
|fontName|String||
|fontSize|Int32||
|margin|Int32||
|text|String||
|uiElementName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.addContentHeaderAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.addContentHeaderAction",
  "uiElementName": "String",
  "text": "String",
  "fontName": "String",
  "fontSize": 1024,
  "fontColor": "String",
  "alignment": "String",
  "margin": 1024
}
```

