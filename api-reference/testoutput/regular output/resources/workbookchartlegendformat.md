---
title: "workbookChartLegendFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartLegendFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartLegendFormats](../api/workbookchartlegendformat-list.md)|[workbookChartLegendFormat](../resources/workbookChartLegendFormat.md) collection|List properties and relationships of the [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) objects.|
|[Get workbookChartLegendFormat](../api/workbookchartlegendformat-get.md)|[workbookChartLegendFormat](../resources/workbookChartLegendFormat.md)|Read properties and relationships of the [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Create workbookChartLegendFormat](../api/workbookchartlegendformat-create.md)|[workbookChartLegendFormat](../resources/workbookChartLegendFormat.md)|Create a new [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Delete workbookChartLegendFormat](../api/workbookchartlegendformat-delete.md)|None|Deletes a [workbookChartLegendFormat](../resources/workbookchartlegendformat.md).|
|[Update workbookChartLegendFormat](../api/workbookchartlegendformat-update.md)|[workbookChartLegendFormat](../resources/workbookChartLegendFormat.md)|Update the properties of a [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookChartFill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookChartFont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookChartFill.md)||
|font|[workbookChartFont](../resources/workbookChartFont.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLegendFormat",
  "id": "String (identifier)"
}
```

