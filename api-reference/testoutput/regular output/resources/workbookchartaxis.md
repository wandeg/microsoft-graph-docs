---
title: "workbookChartAxis resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartAxis resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartAxises](../api/workbookchartaxis-list.md)|[workbookChartAxis](../resources/workbookChartAxis.md) collection|List properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) objects.|
|[Get workbookChartAxis](../api/workbookchartaxis-get.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Read properties and relationships of the [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Create workbookChartAxis](../api/workbookchartaxis-create.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Create a new [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Delete workbookChartAxis](../api/workbookchartaxis-delete.md)|None|Deletes a [workbookChartAxis](../resources/workbookchartaxis.md).|
|[Update workbookChartAxis](../api/workbookchartaxis-update.md)|[workbookChartAxis](../resources/workbookChartAxis.md)|Update the properties of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Get workbookChartAxisFormat](../api/workbookchartaxisformat-get.md)|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md)|Read properties and relationships of the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartAxisTitle](../api/workbookchartaxistitle-get.md)|[workbookChartAxisTitle](../resources/workbookChartAxisTitle.md)|Read properties and relationships of the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|majorUnit|[Json](../resources/Json.md)||
|maximum|[Json](../resources/Json.md)||
|minimum|[Json](../resources/Json.md)||
|minorUnit|[Json](../resources/Json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md)||
|majorGridlines|[workbookChartGridlines](../resources/workbookChartGridlines.md)||
|minorGridlines|[workbookChartGridlines](../resources/workbookChartGridlines.md)||
|title|[workbookChartAxisTitle](../resources/workbookChartAxisTitle.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxis",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "id": "String (identifier)",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

