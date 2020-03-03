---
title: "outlookItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# outlookItem resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List outlookItems](../api/outlookitem-list.md)|[outlookItem](../resources/outlookItem.md) collection|List properties and relationships of the [outlookItem](../resources/outlookitem.md) objects.|
|[Get outlookItem](../api/outlookitem-get.md)|[outlookItem](../resources/outlookItem.md)|Read properties and relationships of the [outlookItem](../resources/outlookitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categories|String collection||
|changeKey|String||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ]
}
```

