---
title: "printerShare resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerShare resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printerShare](../api/printershare-get.md)|[printerShare](../resources/printershare.md)|Read properties and relationships of the [printerShare](../resources/printershare.md) object.|
|[Update printerShare](../api/printershare-update.md)|[printerShare](../resources/printershare.md)|Update the properties of a [printerShare](../resources/printershare.md) object.|
|[Get printer](../api/printer-get.md)|[printer](../resources/printer.md)|Read properties and relationships of the [printer](../resources/printer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|printer|[printer](../resources/printer.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerShare",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

