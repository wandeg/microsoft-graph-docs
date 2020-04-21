---
title: "workbookChartLegend resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartLegend resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartLegend](../api/workbookchartlegend-get.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Read properties and relationships of a [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[Update workbookChartLegend](../api/workbookchartlegend-update.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Update the properties of a [workbookChartLegend](../resources/workbookchartlegend.md) object.|
|[List format](../api/workbookchartlegend-list-format.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md) collection|Get the workbookChartLegendFormats from the format navigation property.|
|[Create format](../api/workbookchartlegend-post-format.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartlegend-delete-format.md)|None|Delete a format object.|
|[Update format](../api/workbookchartlegend-update-format.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Update the properties of a format object.|
|[Get workbookChartLegendFormat](../api/workbookchartlegendformat-get.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Read properties and relationships of a [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[List legend](../api/workbookchart-list-legend.md)|[workbookChartLegend](../resources/workbookchartlegend.md) collection|Get the workbookChartLegends from the legend navigation property.|
|[Create legend](../api/workbookchart-post-legend.md)|[workbookChartLegend](../resources/workbookchartlegend.md)|Create a new legend object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|overlay|Boolean|**TODO: Add Description**|
|position|String|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartLegend",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLegend",
  "id": "String (identifier)",
  "overlay": true,
  "position": "String",
  "visible": true
}
```

