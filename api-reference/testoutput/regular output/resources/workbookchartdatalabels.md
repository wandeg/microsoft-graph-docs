---
title: "workbookChartDataLabels resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartDataLabels resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartDataLabelses](../api/workbookchartdatalabels-list.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md) collection|List properties and relationships of the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) objects.|
|[Get workbookChartDataLabels](../api/workbookchartdatalabels-get.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Read properties and relationships of the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Create workbookChartDataLabels](../api/workbookchartdatalabels-create.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Create a new [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Delete workbookChartDataLabels](../api/workbookchartdatalabels-delete.md)|None|Deletes a [workbookChartDataLabels](../resources/workbookchartdatalabels.md).|
|[Update workbookChartDataLabels](../api/workbookchartdatalabels-update.md)|[workbookChartDataLabels](../resources/workbookchartdatalabels.md)|Update the properties of a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.|
|[Get workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-get.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Read properties and relationships of the [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|position|String||
|separator|String||
|showBubbleSize|Boolean||
|showCategoryName|Boolean||
|showLegendKey|Boolean||
|showPercentage|Boolean||
|showSeriesName|Boolean||
|showValue|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)||

## JSON Representation
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

