---
title: "workbookRangeBorder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookRangeBorder resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookRangeBorder](../api/workbookrangeborder-get.md)|[workbookRangeBorder](../resources/workbookRangeBorder.md)|Read properties and relationships of the [workbookRangeBorder](../resources/workbookrangeborder.md) object.|
|[Delete workbookRangeBorder](../api/workbookrangeborder-delete.md)|None|Deletes a [workbookRangeBorder](../resources/workbookrangeborder.md).|
|[Update workbookRangeBorder](../api/workbookrangeborder-update.md)|[workbookRangeBorder](../resources/workbookRangeBorder.md)|Update the properties of a [workbookRangeBorder](../resources/workbookrangeborder.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|sideIndex|String||
|style|String||
|weight|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "id": "String (identifier)",
  "color": "String",
  "sideIndex": "String",
  "style": "String",
  "weight": "String"
}
```

