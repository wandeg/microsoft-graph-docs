---
title: "workbookChartPointFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartPointFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartPointFormats](../api/workbookchartpointformat-list.md)|[workbookChartPointFormat](../resources/workbookChartPointFormat.md) collection|List properties and relationships of the [workbookChartPointFormat](../resources/workbookchartpointformat.md) objects.|
|[Get workbookChartPointFormat](../api/workbookchartpointformat-get.md)|[workbookChartPointFormat](../resources/workbookChartPointFormat.md)|Read properties and relationships of the [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Create workbookChartPointFormat](../api/workbookchartpointformat-create.md)|[workbookChartPointFormat](../resources/workbookChartPointFormat.md)|Create a new [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Delete workbookChartPointFormat](../api/workbookchartpointformat-delete.md)|None|Deletes a [workbookChartPointFormat](../resources/workbookchartpointformat.md).|
|[Update workbookChartPointFormat](../api/workbookchartpointformat-update.md)|[workbookChartPointFormat](../resources/workbookChartPointFormat.md)|Update the properties of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Get workbookChartFill](../api/workbookchartfill-get.md)|[workbookChartFill](../resources/workbookChartFill.md)|Read properties and relationships of the [workbookChartFill](../resources/workbookchartfill.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fill|[workbookChartFill](../resources/workbookChartFill.md)||

## JSON Representation
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

