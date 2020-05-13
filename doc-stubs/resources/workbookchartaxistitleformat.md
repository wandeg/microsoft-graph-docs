---
title: "workbookChartAxisTitleFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartAxisTitleFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List format](../api/workbookchartaxistitle-list-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) collection|Get the workbookChartAxisTitleFormats from the format navigation property.|
|[Create format](../api/workbookchartaxistitle-post-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartaxistitle-delete-format.md)|None|Delete a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[Update format](../api/workbookchartaxistitle-update-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartaxistitle-get-workbookchartaxistitleformat.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Read the properties and relationships of a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[List font](../api/workbookchartaxistitleformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookchartaxistitleformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookchartaxistitleformat-delete-font.md)|None|Delete a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Update font](../api/workbookchartaxistitleformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get font](../api/workbookchartaxistitleformat-get-workbookchartfont.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read the properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|font|[workbookChartFont](../resources/workbookchartfont.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitleFormat",
  "id": "String (identifier)"
}
```

