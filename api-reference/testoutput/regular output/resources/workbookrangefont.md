---
title: "workbookRangeFont resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookRangeFont resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRangeFonts](../api/workbookrangefont-list.md)|[workbookRangeFont](../resources/workbookRangeFont.md) collection|List properties and relationships of the [workbookRangeFont](../resources/workbookrangefont.md) objects.|
|[Get workbookRangeFont](../api/workbookrangefont-get.md)|[workbookRangeFont](../resources/workbookRangeFont.md)|Read properties and relationships of the [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[Create workbookRangeFont](../api/workbookrangefont-create.md)|[workbookRangeFont](../resources/workbookRangeFont.md)|Create a new [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[Delete workbookRangeFont](../api/workbookrangefont-delete.md)|None|Deletes a [workbookRangeFont](../resources/workbookrangefont.md).|
|[Update workbookRangeFont](../api/workbookrangefont-update.md)|[workbookRangeFont](../resources/workbookRangeFont.md)|Update the properties of a [workbookRangeFont](../resources/workbookrangefont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bold|Boolean||
|color|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|italic|Boolean||
|name|String||
|size|Double||
|underline|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeFont",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeFont",
  "id": "String (identifier)",
  "bold": true,
  "color": "String",
  "italic": true,
  "name": "String",
  "size": "Double",
  "underline": "String"
}
```

