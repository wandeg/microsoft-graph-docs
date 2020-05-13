---
title: "workbookChartTitle resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartTitle resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List title](../api/workbookchart-list-title.md)|[workbookChartTitle](../resources/workbookcharttitle.md) collection|Get the workbookChartTitles from the title navigation property.|
|[Create title](../api/workbookchart-post-title.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Create a new title object.|
|[Delete title](../api/workbookchart-delete-title.md)|None|Delete a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[Update title](../api/workbookchart-update-title.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Update the properties of a title object.|
|[Get title](../api/workbookchart-get-workbookcharttitle.md)|[workbookChartTitle](../resources/workbookcharttitle.md)|Read the properties and relationships of a [workbookChartTitle](../resources/workbookcharttitle.md) object.|
|[List format](../api/workbookcharttitle-list-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md) collection|Get the workbookChartTitleFormats from the format navigation property.|
|[Create format](../api/workbookcharttitle-post-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Create a new format object.|
|[Delete format](../api/workbookcharttitle-delete-format.md)|None|Delete a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|
|[Update format](../api/workbookcharttitle-update-format.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookcharttitle-get-workbookcharttitleformat.md)|[workbookChartTitleFormat](../resources/workbookcharttitleformat.md)|Read the properties and relationships of a [workbookChartTitleFormat](../resources/workbookcharttitleformat.md) object.|

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
The following is a JSON representation of the resource.
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
  "overlay": "Boolean",
  "text": "String",
  "visible": "Boolean"
}
```

