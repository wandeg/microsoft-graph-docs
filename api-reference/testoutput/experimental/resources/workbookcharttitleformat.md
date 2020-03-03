---
title: "workbookChartTitleFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartTitleFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartTitleFormats](../api/workbookcharttitleformat-list.md)|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md) collection|List properties and relationships of the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) objects.|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md)|Read properties and relationships of the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Create workbookChartTitleFormat](../api/workbookcharttitleformat-create.md)|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md)|Create a new [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Delete workbookChartTitleFormat](../api/workbookcharttitleformat-delete.md)|None|Deletes a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md).|
|[Update workbookChartTitleFormat](../api/workbookcharttitleformat-update.md)|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md)|Update the properties of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookChartFill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookChartFont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookChartFill.md)||
|font|[workbookChartFont](../resources/workbookChartFont.md)||

## JSON Representation
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

