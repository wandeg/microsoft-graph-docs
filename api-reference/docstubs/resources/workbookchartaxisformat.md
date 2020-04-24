---
title: "workbookChartAxisFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartAxisFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartAxisFormat](../api/workbookchartaxisformat-get.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Read the properties and relationships of a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Update workbookChartAxisFormat](../api/workbookchartaxisformat-update.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Update the properties of a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[List font](../api/workbookchartaxisformat-list-font.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|Get the workbookChartFonts from the font navigation property.|
|[Create font](../api/workbookchartaxisformat-post-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new font object.|
|[Delete font](../api/workbookchartaxisformat-delete-font.md)|None|Delete a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Update font](../api/workbookchartaxisformat-update-font.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a font object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read the properties and relationships of a [workbookChartFont](../resources/workbookchartfont.md) object.|
|[List line](../api/workbookchartaxisformat-list-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md) collection|Get the workbookChartLineFormats from the line navigation property.|
|[Create line](../api/workbookchartaxisformat-post-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Create a new line object.|
|[Delete line](../api/workbookchartaxisformat-delete-line.md)|None|Delete a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[Update line](../api/workbookchartaxisformat-update-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Update the properties of a line object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read the properties and relationships of a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|font|[workbookChartFont](../resources/workbookchartfont.md)|**TODO: Add Description**|
|line|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisFormat",
  "id": "String (identifier)"
}
```

