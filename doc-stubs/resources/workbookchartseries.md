---
title: "workbookChartSeries resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartSeries resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List series](../api/workbookchart-list-series.md)|[workbookChartSeries](../resources/workbookchartseries.md) collection|Get the workbookChartSeries from the series navigation property.|
|[Create series](../api/workbookchart-post-series.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Create a new series object.|
|[Delete series](../api/workbookchart-delete-series.md)|None|Delete a [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[Update series](../api/workbookchart-update-series.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Update the properties of a series object.|
|[Get series](../api/workbookchart-get-workbookchartseries.md)|[workbookChartSeries](../resources/workbookchartseries.md)|Read the properties and relationships of a [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[itemAt](../api/workbookchartseries-itemat.md)|[workbookChartSeries](../resources/workbookchartseries.md)|**TODO: Add Description**|
|[count](../api/workbookchartseries-count.md)|Int32|**TODO: Add Description**|
|[List format](../api/workbookchartseries-list-format.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) collection|Get the workbookChartSeriesFormats from the format navigation property.|
|[Create format](../api/workbookchartseries-post-format.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartseries-delete-format.md)|None|Delete a [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[Update format](../api/workbookchartseries-update-format.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartseries-get-workbookchartseriesformat.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Read the properties and relationships of a [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[List points](../api/workbookchartseries-list-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md) collection|Get the workbookChartPoints from the points navigation property.|
|[Create points](../api/workbookchartseries-post-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Create a new points object.|
|[Delete points](../api/workbookchartseries-delete-points.md)|None|Delete a [workbookChartPoint](../resources/workbookchartpoint.md) object.|
|[Update points](../api/workbookchartseries-update-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Update the properties of a points object.|
|[Get points](../api/workbookchartseries-get-workbookchartpoint.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Read the properties and relationships of a [workbookChartPoint](../resources/workbookchartpoint.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|**TODO: Add Description**|
|points|[workbookChartPoint](../resources/workbookchartpoint.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartSeries",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartSeries",
  "id": "String (identifier)",
  "name": "String"
}
```

