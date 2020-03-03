---
title: "workbookChartAxisTitle resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartAxisTitle resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartAxisTitles](../api/workbookchartaxistitle-list.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md) collection|List properties and relationships of the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) objects.|
|[Get workbookChartAxisTitle](../api/workbookchartaxistitle-get.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Read properties and relationships of the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[Create workbookChartAxisTitle](../api/workbookchartaxistitle-create.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Create a new [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[Delete workbookChartAxisTitle](../api/workbookchartaxistitle-delete.md)|None|Deletes a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md).|
|[Update workbookChartAxisTitle](../api/workbookchartaxistitle-update.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Update the properties of a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[Get workbookChartAxisTitleFormat](../api/workbookchartaxistitleformat-get.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Read properties and relationships of the [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxisTitle",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "id": "String (identifier)",
  "text": "String",
  "visible": true
}
```

