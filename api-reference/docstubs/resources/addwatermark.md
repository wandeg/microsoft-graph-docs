---
title: "addWatermark resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# addWatermark resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [markContent](../resources/markcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fontColor|String|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md)|
|fontSize|Int64|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md)|
|name|String|**TODO: Add Description** Inherited from [labelActionBase](../resources/labelactionbase.md)|
|orientation|pageOrientation|**TODO: Add Description**. Possible values are: `horizontal`, `diagonal`.|
|text|String|**TODO: Add Description** Inherited from [markContent](../resources/markcontent.md)|

## Relationships
None

## JSON representation
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

