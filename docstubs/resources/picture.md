---
title: "picture resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# picture resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read properties and relationships of the [picture](../resources/picture.md) object.|
|[Update picture](../api/picture-update.md)|[picture](../resources/picture.md)|Update the properties of a [picture](../resources/picture.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|contentType|String||
|height|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|width|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.picture",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.picture",
  "id": "String (identifier)",
  "width": 1024,
  "height": 1024,
  "contentType": "String",
  "content": "Stream"
}
```

