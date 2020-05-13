---
title: "workbookChartTitleFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartTitleFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List format](../api/workbookcharttitle-list-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md) collection|Get the workbookChartTitleFormats from the format navigation property.|
|[Create format](../api/workbookcharttitle-post-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Create a new format object.|
|[Delete format](../api/workbookcharttitle-delete-format.md)|None|Delete a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Update format](../api/workbookcharttitle-update-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookcharttitle-get-workbookcharttitleformat.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read the properties and relationships of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[List fill](../api/workbookcharttitleformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookcharttitleformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookcharttitleformat-delete-fill.md)|None|Delete a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Update fill](../api/workbookcharttitleformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get fill](../api/workbookcharttitleformat-get-workbookchartfill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read the properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List font](../api/workbookcharttitleformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookcharttitleformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookcharttitleformat-delete-font.md)|None|Delete a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Update font](../api/workbookcharttitleformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get font](../api/workbookcharttitleformat-get-workbookchartfont.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read the properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|

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
The following is a JSON representation of the resource.
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

