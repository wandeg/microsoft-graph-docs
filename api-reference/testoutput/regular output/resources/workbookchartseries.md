---
title: "workbookChartSeries resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartSeries resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartSeries](../api/workbookchartseries-get.md)|[workbookChartSeries](../resources/workbookChartSeries.md)|Read properties and relationships of the [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[Delete workbookChartSeries](../api/workbookchartseries-delete.md)|None|Deletes a [workbookChartSeries](../resources/workbookchartseries.md).|
|[Update workbookChartSeries](../api/workbookchartseries-update.md)|[workbookChartSeries](../resources/workbookChartSeries.md)|Update the properties of a [workbookChartSeries](../resources/workbookchartseries.md) object.|
|[Get workbookChartSeriesFormat](../api/workbookchartseriesformat-get.md)|[workbookChartSeriesFormat](../resources/workbookChartSeriesFormat.md)|Read properties and relationships of the [workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) object.|
|[List points](../api/workbookchartseries-list-points.md)|[workbookChartPoint](../resources/workbookChartPoint.md) collection|Get the workbookChartPoints from the points navigation property.|
|[Add points](../api/workbookchartseries-post-points.md)|[workbookChartPoint](../resources/workbookChartPoint.md)|Add points by posting to the points collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartSeriesFormat](../resources/workbookChartSeriesFormat.md)||
|points|[workbookChartPoint](../resources/workbookChartPoint.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

