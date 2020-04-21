---
title: "workbookChartPointFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartPointFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartPointFormat](../api/workbookchartpointformat-get.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Read properties and relationships of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Update workbookChartPointFormat](../api/workbookchartpointformat-update.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Update the properties of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[List fill](../api/workbookchartpointformat-list-fill.md)|[workbookChartFill](../resources/workbookchartfill.md) collection|Get the workbookChartFills from the fill navigation property.|
|[Create fill](../api/workbookchartpointformat-post-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Create a new fill object.|
|[Delete fill](../api/workbookchartpointformat-delete-fill.md)|None|Delete a fill object.|
|[Update fill](../api/workbookchartpointformat-update-fill.md)|[workbookChartFill](../resources/workbookchartfill.md)|Update the properties of a fill object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookchartfill.md)|Read properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.|
|[List format](../api/workbookchartpoint-list-format.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md) collection|Get the workbookChartPointFormats from the format navigation property.|
|[Create format](../api/workbookchartpoint-post-format.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Create a new format object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookchartfill.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartPointFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartPointFormat",
  "id": "String (identifier)"
}
```

