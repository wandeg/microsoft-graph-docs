---
title: "workbookChartAxisFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartAxisFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartAxisFormats](../api/workbookchartaxisformat-list.md)|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md) collection|List properties and relationships of the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) objects.|
|[Get workbookChartAxisFormat](../api/workbookchartaxisformat-get.md)|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md)|Read properties and relationships of the [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Create workbookChartAxisFormat](../api/workbookchartaxisformat-create.md)|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md)|Create a new [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Delete workbookChartAxisFormat](../api/workbookchartaxisformat-delete.md)|None|Deletes a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md).|
|[Update workbookChartAxisFormat](../api/workbookchartaxisformat-update.md)|[workbookChartAxisFormat](../resources/workbookChartAxisFormat.md)|Update the properties of a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookChartFont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookChartLineFormat.md)|Read properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|font|[workbookChartFont](../resources/workbookChartFont.md)||
|line|[workbookChartLineFormat](../resources/workbookChartLineFormat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisFormat",
  "id": "String (identifier)"
}
```

