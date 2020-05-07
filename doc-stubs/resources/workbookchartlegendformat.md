---
title: "workbookChartLegendFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartLegendFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List fill](../api/workbookchartlegendformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookchartlegendformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookchartlegendformat-delete-fill.md)|None|Delete a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Update fill](../api/workbookchartlegendformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read the properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List font](../api/workbookchartlegendformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookchartlegendformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookchartlegendformat-delete-font.md)|None|Delete a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Update font](../api/workbookchartlegendformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read the properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[List format](../api/workbookchartlegend-list-format.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md) collection|Get the workbookChartLegendFormats from the format navigation property.|
|[Create format](../api/workbookchartlegend-post-format.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Create a new format object.|

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
  "@odata.type": "microsoft.graph.workbookChartLegendFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLegendFormat",
  "id": "String (identifier)"
}
```

