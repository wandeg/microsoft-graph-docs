---
title: "workbookChartDataLabels resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartDataLabels resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartDataLabels](../api/workbookchartdatalabels-get.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Read properties and relationships of a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Update workbookChartDataLabels](../api/workbookchartdatalabels-update.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Update the properties of a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[List format](../api/workbookchartdatalabels-list-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) collection|Get the workbookChartDataLabelFormats from the format navigation property.|
|[Create format](../api/workbookchartdatalabels-post-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartdatalabels-delete-format.md)|None|Delete a format object.|
|[Update format](../api/workbookchartdatalabels-update-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Update the properties of a format object.|
|[Get workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-get.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Read properties and relationships of a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[List dataLabels](../api/workbookchart-list-datalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md) collection|Get the workbookChartDataLabels from the dataLabels navigation property.|
|[Create dataLabels](../api/workbookchart-post-datalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Create a new dataLabels object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|position|String|**TODO: Add Description**|
|separator|String|**TODO: Add Description**|
|showBubbleSize|Boolean|**TODO: Add Description**|
|showCategoryName|Boolean|**TODO: Add Description**|
|showLegendKey|Boolean|**TODO: Add Description**|
|showPercentage|Boolean|**TODO: Add Description**|
|showSeriesName|Boolean|**TODO: Add Description**|
|showValue|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartDataLabels",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartDataLabels",
  "id": "String (identifier)",
  "position": "String",
  "separator": "String",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}
```

