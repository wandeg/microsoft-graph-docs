---
title: "workbookChartDataLabels resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartDataLabels resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List dataLabels](../api/workbookchart-list-datalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md) collection|Get the workbookChartDataLabels from the dataLabels navigation property.|
|[Create dataLabels](../api/workbookchart-post-datalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Create a new dataLabels object.|
|[Delete dataLabels](../api/workbookchart-delete-datalabels.md)|None|Delete a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Update dataLabels](../api/workbookchart-update-datalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Update the properties of a dataLabels object.|
|[Get dataLabels](../api/workbookchart-get-workbookchartdatalabels.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Read the properties and relationships of a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[List format](../api/workbookchartdatalabels-list-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) collection|Get the workbookChartDataLabelFormats from the format navigation property.|
|[Create format](../api/workbookchartdatalabels-post-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartdatalabels-delete-format.md)|None|Delete a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[Update format](../api/workbookchartdatalabels-update-format.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartdatalabels-get-workbookchartdatalabelformat.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Read the properties and relationships of a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|

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
The following is a JSON representation of the resource.
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
  "showBubbleSize": "Boolean",
  "showCategoryName": "Boolean",
  "showLegendKey": "Boolean",
  "showPercentage": "Boolean",
  "showSeriesName": "Boolean",
  "showValue": "Boolean"
}
```

