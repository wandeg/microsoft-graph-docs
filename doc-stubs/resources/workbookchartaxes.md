---
title: "workbookChartAxes resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartAxes resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List axes](../api/workbookchart-list-axes.md)|[workbookChartAxes](../resources/workbookchartaxes.md) collection|Get the workbookChartAxes from the axes navigation property.|
|[Create axes](../api/workbookchart-post-axes.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Create a new axes object.|
|[Delete axes](../api/workbookchart-delete-axes.md)|None|Delete a [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[Update axes](../api/workbookchart-update-axes.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Update the properties of an axes object.|
|[Get axes](../api/workbookchart-get-workbookchartaxes.md)|[workbookChartAxes](../resources/workbookchartaxes.md)|Read the properties and relationships of a [workbookChartAxes](../resources/workbookchartaxes.md) object.|
|[List categoryAxis](../api/workbookchartaxes-list-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md) collection|Get the workbookChartAxis from the categoryAxis navigation property.|
|[Create categoryAxis](../api/workbookchartaxes-post-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Create a new categoryAxis object.|
|[Delete categoryAxis](../api/workbookchartaxes-delete-categoryaxis.md)|None|Delete a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Update categoryAxis](../api/workbookchartaxes-update-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Update the properties of a categoryAxis object.|
|[Get categoryAxis](../api/workbookchartaxes-get-workbookchartaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read the properties and relationships of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[List seriesAxis](../api/workbookchartaxes-list-seriesaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md) collection|Get the workbookChartAxis from the seriesAxis navigation property.|
|[Create seriesAxis](../api/workbookchartaxes-post-seriesaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Create a new seriesAxis object.|
|[Delete seriesAxis](../api/workbookchartaxes-delete-seriesaxis.md)|None|Delete a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Update seriesAxis](../api/workbookchartaxes-update-seriesaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Update the properties of a seriesAxis object.|
|[Get seriesAxis](../api/workbookchartaxes-get-workbookchartaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read the properties and relationships of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[List valueAxis](../api/workbookchartaxes-list-valueaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md) collection|Get the workbookChartAxis from the valueAxis navigation property.|
|[Create valueAxis](../api/workbookchartaxes-post-valueaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Create a new valueAxis object.|
|[Delete valueAxis](../api/workbookchartaxes-delete-valueaxis.md)|None|Delete a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Update valueAxis](../api/workbookchartaxes-update-valueaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Update the properties of a valueAxis object.|
|[Get valueAxis](../api/workbookchartaxes-get-workbookchartaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read the properties and relationships of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categoryAxis|[workbookChartAxis](../resources/workbookchartaxis.md)|**TODO: Add Description**|
|seriesAxis|[workbookChartAxis](../resources/workbookchartaxis.md)|**TODO: Add Description**|
|valueAxis|[workbookChartAxis](../resources/workbookchartaxis.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

