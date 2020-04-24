---
title: "addWatermarkAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# addWatermarkAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fontColor|String|**TODO: Add Description**|
|fontName|String|**TODO: Add Description**|
|fontSize|Int32|**TODO: Add Description**|
|layout|watermarkLayout|**TODO: Add Description**. Possible values are: `horizontal`, `diagonal`.|
|text|String|**TODO: Add Description**|
|uiElementName|String|**TODO: Add Description**|

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

