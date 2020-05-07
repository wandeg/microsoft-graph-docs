---
title: "workbookChartSeriesFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartSeriesFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List fill](../api/workbookchartseriesformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookchartseriesformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookchartseriesformat-delete-fill.md)|None|Delete a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[Update fill](../api/workbookchartseriesformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read the properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List line](../api/workbookchartseriesformat-list-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md) collection|Get the workbookChartLineFormats from the line navigation property.|
|[Create line](../api/workbookchartseriesformat-post-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Create a new line object.|
|[Delete line](../api/workbookchartseriesformat-delete-line.md)|None|Delete a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[Update line](../api/workbookchartseriesformat-update-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Update the properties of a line object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read the properties and relationships of a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[List format](../api/workbookchartseries-list-format.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md) collection|Get the workbookChartSeriesFormats from the format navigation property.|
|[Create format](../api/workbookchartseries-post-format.md)|[workbookChartSeriesFormat](../resources/workbookchartseriesformat.md)|Create a new format object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)|**TODO: Add Description**|
|line|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartSeriesFormat",
  "id": "String (identifier)"
}
```

