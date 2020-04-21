---
title: "workbookChartTitleFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartTitleFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read properties and relationships of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Update workbookChartTitleFormat](../api/workbookcharttitleformat-update.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Update the properties of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[List fill](../api/workbookcharttitleformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookcharttitleformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookcharttitleformat-delete-fill.md)|None|Delete a fill object.|
|[Update fill](../api/workbookcharttitleformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List font](../api/workbookcharttitleformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookcharttitleformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookcharttitleformat-delete-font.md)|None|Delete a font object.|
|[Update font](../api/workbookcharttitleformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[List format](../api/workbookcharttitle-list-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md) collection|Get the workbookChartTitleFormats from the format navigation property.|
|[Create format](../api/workbookcharttitle-post-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Create a new format object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)|**TODO: Add Description**|
|font|[workbookChartFont](../resources/workbookchartfont.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartTitleFormat",
  "id": "String (identifier)"
}
```

