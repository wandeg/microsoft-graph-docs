---
title: "workbookChartDataLabelFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartDataLabelFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartDataLabelFormats](../api/workbookchartdatalabelformat-list.md)|[workbookChartDataLabelFormat](../resources/workbookChartDataLabelFormat.md) collection|List properties and relationships of the [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) objects.|
|[Get workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-get.md)|[workbookChartDataLabelFormat](../resources/workbookChartDataLabelFormat.md)|Read properties and relationships of the [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[Create workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-create.md)|[workbookChartDataLabelFormat](../resources/workbookChartDataLabelFormat.md)|Create a new [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[Delete workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-delete.md)|None|Deletes a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md).|
|[Update workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-update.md)|[workbookChartDataLabelFormat](../resources/workbookChartDataLabelFormat.md)|Update the properties of a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
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
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartDataLabelFormat",
  "id": "String (identifier)"
}
```

