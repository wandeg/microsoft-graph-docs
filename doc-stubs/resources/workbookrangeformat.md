---
title: "workbookRangeFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookRangeFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List format](../api/workbookrange-list-format.md)|[workbookRangeFormat](../resources/workbookrangeformat.md) collection|Get the workbookRangeFormats from the format navigation property.|
|[Create format](../api/workbookrange-post-format.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Create a new format object.|
|[Delete format](../api/workbookrange-delete-format.md)|None|Delete a [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Update format](../api/workbookrange-update-format.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookrange-get-workbookrangeformat.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Read the properties and relationships of a [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[autofitColumns](../api/workbookrangeformat-autofitcolumns.md)|None|**TODO: Add Description**|
|[autofitRows](../api/workbookrangeformat-autofitrows.md)|None|**TODO: Add Description**|
|[List borders](../api/workbookrangeformat-list-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md) collection|Get the workbookRangeBorders from the borders navigation property.|
|[Create borders](../api/workbookrangeformat-post-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Create a new borders object.|
|[Delete borders](../api/workbookrangeformat-delete-borders.md)|None|Delete a [workbookRangeBorder](../resources/workbookrangeborder.md) object.|
|[Update borders](../api/workbookrangeformat-update-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Update the properties of a borders object.|
|[Get borders](../api/workbookrangeformat-get-workbookrangeborder.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Read the properties and relationships of a [workbookRangeBorder](../resources/workbookrangeborder.md) object.|
|[List fill](../api/workbookrangeformat-list-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md) collection|Get the workbookRangeFills from the fill navigation property.|
|[Create fill](../api/workbookrangeformat-post-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Create a new fill object.|
|[Delete fill](../api/workbookrangeformat-delete-fill.md)|None|Delete a [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Update fill](../api/workbookrangeformat-update-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Update the properties of a fill object.|
|[Get fill](../api/workbookrangeformat-get-workbookrangefill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Read the properties and relationships of a [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[List font](../api/workbookrangeformat-list-font.md)|[workbookRangeFont](../resources/workbookrangefont.md) collection|Get the workbookRangeFonts from the font navigation property.|
|[Create font](../api/workbookrangeformat-post-font.md)|[workbookRangeFont](../resources/workbookrangefont.md)|Create a new font object.|
|[Delete font](../api/workbookrangeformat-delete-font.md)|None|Delete a [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[Update font](../api/workbookrangeformat-update-font.md)|[workbookRangeFont](../resources/workbookrangefont.md)|Update the properties of a font object.|
|[Get font](../api/workbookrangeformat-get-workbookrangefont.md)|[workbookRangeFont](../resources/workbookrangefont.md)|Read the properties and relationships of a [workbookRangeFont](../resources/workbookrangefont.md) object.|
|[List protection](../api/workbookrangeformat-list-protection.md)|[workbookFormatProtection](../resources/workbookformatprotection.md) collection|Get the workbookFormatProtections from the protection navigation property.|
|[Create protection](../api/workbookrangeformat-post-protection.md)|[workbookFormatProtection](../resources/workbookformatprotection.md)|Create a new protection object.|
|[Delete protection](../api/workbookrangeformat-delete-protection.md)|None|Delete a [workbookFormatProtection](../resources/workbookformatprotection.md) object.|
|[Update protection](../api/workbookrangeformat-update-protection.md)|[workbookFormatProtection](../resources/workbookformatprotection.md)|Update the properties of a protection object.|
|[Get protection](../api/workbookrangeformat-get-workbookformatprotection.md)|[workbookFormatProtection](../resources/workbookformatprotection.md)|Read the properties and relationships of a [workbookFormatProtection](../resources/workbookformatprotection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|columnWidth|Double|**TODO: Add Description**|
|horizontalAlignment|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|rowHeight|Double|**TODO: Add Description**|
|verticalAlignment|String|**TODO: Add Description**|
|wrapText|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|borders|[workbookRangeBorder](../resources/workbookrangeborder.md) collection|**TODO: Add Description**|
|fill|[workbookRangeFill](../resources/workbookrangefill.md)|**TODO: Add Description**|
|font|[workbookRangeFont](../resources/workbookrangefont.md)|**TODO: Add Description**|
|protection|[workbookFormatProtection](../resources/workbookformatprotection.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "wrapText": "Boolean"
}
```

