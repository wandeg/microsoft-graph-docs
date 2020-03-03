---
title: "workbookChart resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChart resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChart](../api/workbookchart-get.md)|[workbookChart](../resources/workbookChart.md)|Read properties and relationships of the [workbookChart](../resources/workbookchart.md) object.|
|[Delete workbookChart](../api/workbookchart-delete.md)|None|Deletes a [workbookChart](../resources/workbookchart.md).|
|[Update workbookChart](../api/workbookchart-update.md)|[workbookChart](../resources/workbookChart.md)|Update the properties of a [workbookChart](../resources/workbookchart.md) object.|
|[Get workbookChartAxes](../api/workbookchartaxes-get.md)|[workbookChartAxes](../resources/workbookChartAxes.md)|Read properties and relationships of the [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Get workbookChartDataLabels](../api/workbookchartdatalabels-get.md)|[workbookChartDataLabels](../resources/workbookChartDataLabels.md)|Read properties and relationships of the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Get workbookChartAreaFormat](../api/workbookchartareaformat-get.md)|[workbookChartAreaFormat](../resources/workbookChartAreaFormat.md)|Read properties and relationships of the [workbookChartAreaFormat](../resources/workbookchartareaformat.md) object.|
|[Get workbookChartLegend](../api/workbookchartlegend-get.md)|[workbookChartLegend](../resources/workbookChartLegend.md)|Read properties and relationships of the [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[List series](../api/workbookchart-list-series.md)|[workbookChartSeries](../resources/workbookChartSeries.md) collection|Get the workbookChartSerieses from the series navigation property.|
|[Add series](../api/workbookchart-post-series.md)|[workbookChartSeries](../resources/workbookChartSeries.md)|Add series by posting to the series collection.|
|[Get workbookChartTitle](../api/workbookcharttitle-get.md)|[workbookChartTitle](../resources/workbookChartTitle.md)|Read properties and relationships of the [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookWorksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|height|Double||
|id|String| Inherited from [entity](../resources/entity.md)|
|left|Double||
|name|String||
|top|Double||
|width|Double||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|axes|[workbookChartAxes](../resources/workbookChartAxes.md)||
|dataLabels|[workbookChartDataLabels](../resources/workbookChartDataLabels.md)||
|format|[workbookChartAreaFormat](../resources/workbookChartAreaFormat.md)||
|legend|[workbookChartLegend](../resources/workbookChartLegend.md)||
|series|[workbookChartSeries](../resources/workbookChartSeries.md) collection||
|title|[workbookChartTitle](../resources/workbookChartTitle.md)||
|worksheet|[workbookWorksheet](../resources/workbookWorksheet.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChart",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChart",
  "id": "String (identifier)",
  "height": "Double",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
}
```

