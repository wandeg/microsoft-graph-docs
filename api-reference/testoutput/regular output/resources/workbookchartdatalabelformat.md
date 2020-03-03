---
title: "workbookChartDataLabelFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartDataLabelFormat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartDataLabelFormats](../api/workbookchartdatalabelformat-list.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) collection|List properties and relationships of the [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) objects.|
|[Get workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-get.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Read properties and relationships of the [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[Create workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-create.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Create a new [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
|[Delete workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-delete.md)|None|Deletes a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md).|
|[Update workbookChartDataLabelFormat](../api/workbookchartdatalabelformat-update.md)|[workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md)|Update the properties of a [workbookChartDataLabelFormat](../resources/workbookchartdatalabelformat.md) object.|
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

