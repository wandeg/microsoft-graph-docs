---
title: "workbookChartLegendFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartLegendFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartLegendFormats](../api/workbookchartlegendformat-list.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md) collection|List properties and relationships of the [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) objects.|
|[Get workbookChartLegendFormat](../api/workbookchartlegendformat-get.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Read properties and relationships of the [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Create workbookChartLegendFormat](../api/workbookchartlegendformat-create.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Create a new [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Delete workbookChartLegendFormat](../api/workbookchartlegendformat-delete.md)|None|Deletes a [workbookChartLegendFormat](../resources/workbookchartlegendformat.md).|
|[Update workbookChartLegendFormat](../api/workbookchartlegendformat-update.md)|[workbookChartLegendFormat](../resources/workbookchartlegendformat.md)|Update the properties of a [workbookChartLegendFormat](../resources/workbookchartlegendformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)||
|font|[workbookChartFont](../resources/workbookchartfont.md)||

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

