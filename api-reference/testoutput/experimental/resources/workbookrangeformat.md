---
title: "workbookRangeFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookRangeFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRangeFormats](../api/workbookrangeformat-list.md)|[workbookRangeFormat](../resources/workbookRangeFormat.md) collection|List properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) objects.|
|[Get workbookRangeFormat](../api/workbookrangeformat-get.md)|[workbookRangeFormat](../resources/workbookRangeFormat.md)|Read properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Create workbookRangeFormat](../api/workbookrangeformat-create.md)|[workbookRangeFormat](../resources/workbookRangeFormat.md)|Create a new [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Delete workbookRangeFormat](../api/workbookrangeformat-delete.md)|None|Deletes a [workbookRangeFormat](../resources/workbookrangeformat.md).|
|[Update workbookRangeFormat](../api/workbookrangeformat-update.md)|[workbookRangeFormat](../resources/workbookRangeFormat.md)|Update the properties of a [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[List borders](../api/workbookrangeformat-list-borders.md)|[workbookRangeBorder](../resources/workbookRangeBorder.md) collection|Get the workbookRangeBorders from the borders navigation property.|
|[Add borders](../api/workbookrangeformat-post-borders.md)|[workbookRangeBorder](../resources/workbookRangeBorder.md)|Add borders by posting to the borders collection.|
|[Get workbookRangeFill](../api/workbookrangefill-get.md)|[workbookRangeFill](../resources/workbookRangeFill.md)|Read properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Get workbookRangeFont](../api/workbookrangefont-get.md)|[workbookRangeFont](../resources/workbookRangeFont.md)|Read properties and relationships of the [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[Get workbookFormatProtection](../api/workbookformatprotection-get.md)|[workbookFormatProtection](../resources/workbookFormatProtection.md)|Read properties and relationships of the [workbookFormatProtection](../resources/workbookformatprotection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|columnWidth|Double||
|horizontalAlignment|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|rowHeight|Double||
|verticalAlignment|String||
|wrapText|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|borders|[workbookRangeBorder](../resources/workbookRangeBorder.md) collection||
|fill|[workbookRangeFill](../resources/workbookRangeFill.md)||
|font|[workbookRangeFont](../resources/workbookRangeFont.md)||
|protection|[workbookFormatProtection](../resources/workbookFormatProtection.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "id": "String (identifier)",
  "columnWidth": "Double",
  "horizontalAlignment": "String",
  "rowHeight": "Double",
  "verticalAlignment": "String",
  "wrapText": true
}
```

