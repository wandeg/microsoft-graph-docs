---
title: "workbookChartAxisTitle resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartAxisTitle resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List title](../api/workbookchartaxis-list-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md) collection|Get the workbookChartAxisTitles from the title navigation property.|
|[Create title](../api/workbookchartaxis-post-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Create a new title object.|
|[Delete title](../api/workbookchartaxis-delete-title.md)|None|Delete a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[Update title](../api/workbookchartaxis-update-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Update the properties of a title object.|
|[Get title](../api/workbookchartaxis-get-workbookchartaxistitle.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Read the properties and relationships of a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[List format](../api/workbookchartaxistitle-list-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) collection|Get the workbookChartAxisTitleFormats from the format navigation property.|
|[Create format](../api/workbookchartaxistitle-post-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartaxistitle-delete-format.md)|None|Delete a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|
|[Update format](../api/workbookchartaxistitle-update-format.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartaxistitle-get-workbookchartaxistitleformat.md)|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|Read the properties and relationships of a [workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|text|String|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartAxisTitleFormat](../resources/workbookchartaxistitleformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "visible": "Boolean"
}
```

