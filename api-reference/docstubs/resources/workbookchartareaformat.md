---
title: "workbookChartAreaFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartAreaFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAreaFormat](../api/workbookchartareaformat-get.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Read properties and relationships of a [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
|[Update workbookChartAreaFormat](../api/workbookchartareaformat-update.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Update the properties of a [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
|[List fill](../api/workbookchartareaformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookchartareaformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookchartareaformat-delete-fill.md)|None|Delete a fill object.|
|[Update fill](../api/workbookchartareaformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List font](../api/workbookchartareaformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookchartareaformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookchartareaformat-delete-font.md)|None|Delete a font object.|
|[Update font](../api/workbookchartareaformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[List format](../api/workbookchart-list-format.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md) collection|Get the workbookChartAreaFormats from the format navigation property.|
|[Create format](../api/workbookchart-post-format.md)|[workbookChartAreaFormat](../resources/workbookchartareaformat.md)|Create a new format object.|

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
  "@odata.type": "microsoft.graph.workbookChartAreaFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAreaFormat",
  "id": "String (identifier)"
}
```

