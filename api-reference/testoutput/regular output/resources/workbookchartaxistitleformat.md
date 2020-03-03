---
title: "workbookChartAxisTitleFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartAxisTitleFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartAxisTitleFormats](../api/workbookchartaxistitleformat-list.md)|[workbookChartAxisTitleFormat](../resources/workbookChartAxisTitleFormat.md) collection|List properties and relationships of the [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) objects.|
|[Get workbookChartAxisTitleFormat](../api/workbookchartaxistitleformat-get.md)|[workbookChartAxisTitleFormat](../resources/workbookChartAxisTitleFormat.md)|Read properties and relationships of the [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[Create workbookChartAxisTitleFormat](../api/workbookchartaxistitleformat-create.md)|[workbookChartAxisTitleFormat](../resources/workbookChartAxisTitleFormat.md)|Create a new [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[Delete workbookChartAxisTitleFormat](../api/workbookchartaxistitleformat-delete.md)|None|Deletes a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md).|
|[Update workbookChartAxisTitleFormat](../api/workbookchartaxistitleformat-update.md)|[workbookChartAxisTitleFormat](../resources/workbookChartAxisTitleFormat.md)|Update the properties of a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookChartFont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|font|[workbookChartFont](../resources/workbookChartFont.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitleFormat",
  "id": "String (identifier)"
}
```

