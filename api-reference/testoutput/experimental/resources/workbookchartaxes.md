---
title: "workbookChartAxes resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartAxes resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartAxeses](../api/workbookchartaxes-list.md)|[workbookChartAxes](../resources/workbookChartAxes.md) collection|List properties and relationships of the [workbookChartAxes](../resources/workbookchartaxes.md) objects.|
|[Get workbookChartAxes](../api/workbookchartaxes-get.md)|[workbookChartAxes](../resources/workbookChartAxes.md)|Read properties and relationships of the [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Create workbookChartAxes](../api/workbookchartaxes-create.md)|[workbookChartAxes](../resources/workbookChartAxes.md)|Create a new [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Delete workbookChartAxes](../api/workbookchartaxes-delete.md)|None|Deletes a [workbookChartAxes](../resources/workbookchartaxes.md).|
|[Update workbookChartAxes](../api/workbookchartaxes-update.md)|[workbookChartAxes](../resources/workbookChartAxes.md)|Update the properties of a [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categoryAxis|[workbookChartAxis](../resources/workbookChartAxis.md)||
|seriesAxis|[workbookChartAxis](../resources/workbookChartAxis.md)||
|valueAxis|[workbookChartAxis](../resources/workbookChartAxis.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxes",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxes",
  "id": "String (identifier)"
}
```

