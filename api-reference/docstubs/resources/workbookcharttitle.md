---
title: "workbookChartTitle resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartTitle resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartTitle](../api/workbookcharttitle-get.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Read properties and relationships of a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Update workbookChartTitle](../api/workbookcharttitle-update.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Update the properties of a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[List format](../api/workbookcharttitle-list-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md) collection|Get the workbookChartTitleFormats from the format navigation property.|
|[Create format](../api/workbookcharttitle-post-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Create a new format object.|
|[Delete format](../api/workbookcharttitle-delete-format.md)|None|Delete a format object.|
|[Update format](../api/workbookcharttitle-update-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Update the properties of a format object.|
|[Get workbookChartTitleFormat](../api/workbookcharttitleformat-get.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read properties and relationships of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[List title](../api/workbookchart-list-title.md)|[workbookChartTitle](../resources/workbookcharttitle.md) collection|Get the workbookChartTitles from the title navigation property.|
|[Create title](../api/workbookchart-post-title.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Create a new title object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|overlay|Boolean|**TODO: Add Description**|
|text|String|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|**TODO: Add Description**|

## JSON representation
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

