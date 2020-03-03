---
title: "workbookRangeFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookRangeFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRangeFormats](../api/workbookrangeformat-list.md)|[workbookRangeFormat](../resources/workbookrangeformat.md) collection|List properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) objects.|
|[Get workbookRangeFormat](../api/workbookrangeformat-get.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Read properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Create workbookRangeFormat](../api/workbookrangeformat-create.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Create a new [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Delete workbookRangeFormat](../api/workbookrangeformat-delete.md)|None|Deletes a [workbookRangeFormat](../resources/workbookrangeformat.md).|
|[Update workbookRangeFormat](../api/workbookrangeformat-update.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Update the properties of a [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[List borders](../api/workbookrangeformat-list-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md) collection|Get the workbookRangeBorders from the borders navigation property.|
|[Add borders](../api/workbookrangeformat-post-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Add borders by posting to the borders collection.|
|[Get workbookRangeFill](../api/workbookrangefill-get.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Read properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Get workbookRangeFont](../api/workbookrangefont-get.md)|[workbookRangeFont](../resources/workbookrangefont.md)|Read properties and relationships of the [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[Get workbookFormatProtection](../api/workbookformatprotection-get.md)|[workbookFormatProtection](../resources/workbookformatprotection.md)|Read properties and relationships of the [workbookFormatProtection](../resources/workbookformatprotection.md) object.|

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
|borders|[workbookRangeBorder](../resources/workbookrangeborder.md) collection||
|fill|[workbookRangeFill](../resources/workbookrangefill.md)||
|font|[workbookRangeFont](../resources/workbookrangefont.md)||
|protection|[workbookFormatProtection](../resources/workbookformatprotection.md)||

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

