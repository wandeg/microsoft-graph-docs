---
title: "workbookChartTitle resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartTitle resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartTitles](../api/workbookcharttitle-list.md)|[workbookChartTitle](../resources/workbookChartTitle.md) collection|List properties and relationships of the [workbookChartTitle](../resources/workbookcharttitle.md) objects.|
|[Get workbookChartTitle](../api/workbookcharttitle-get.md)|[workbookChartTitle](../resources/workbookChartTitle.md)|Read properties and relationships of the [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Create workbookChartTitle](../api/workbookcharttitle-create.md)|[workbookChartTitle](../resources/workbookChartTitle.md)|Create a new [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Delete workbookChartTitle](../api/workbookcharttitle-delete.md)|None|Deletes a [workbookChartTitle](../resources/workbookcharttitle.md).|
|[Update workbookChartTitle](../api/workbookcharttitle-update.md)|[workbookChartTitle](../resources/workbookChartTitle.md)|Update the properties of a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md)|Read properties and relationships of the [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|overlay|Boolean||
|text|String||
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartTitleFormat](../resources/workbookChartTitleFormat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartTitle",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "id": "String (identifier)",
  "overlay": true,
  "text": "String",
  "visible": true
}
```

