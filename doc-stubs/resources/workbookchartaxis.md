---
title: "workbookChartAxis resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartAxis resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List categoryAxis](../api/workbookchartaxes-list-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md) collection|Get the workbookChartAxis from the categoryAxis navigation property.|
|[Create categoryAxis](../api/workbookchartaxes-post-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Create a new categoryAxis object.|
|[Delete categoryAxis](../api/workbookchartaxes-delete-categoryaxis.md)|None|Delete a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[Update categoryAxis](../api/workbookchartaxes-update-categoryaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Update the properties of a categoryAxis object.|
|[Get categoryAxis](../api/workbookchartaxes-get-workbookchartaxis.md)|[workbookChartAxis](../resources/workbookchartaxis.md)|Read the properties and relationships of a [workbookChartAxis](../resources/workbookchartaxis.md) object.|
|[List format](../api/workbookchartaxis-list-format.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md) collection|Get the workbookChartAxisFormats from the format navigation property.|
|[Create format](../api/workbookchartaxis-post-format.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartaxis-delete-format.md)|None|Delete a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[Update format](../api/workbookchartaxis-update-format.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartaxis-get-workbookchartaxisformat.md)|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|Read the properties and relationships of a [workbookChartAxisFormat](../resources/workbookchartaxisformat.md) object.|
|[List majorGridlines](../api/workbookchartaxis-list-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md) collection|Get the workbookChartGridlines from the majorGridlines navigation property.|
|[Create majorGridlines](../api/workbookchartaxis-post-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Create a new majorGridlines object.|
|[Delete majorGridlines](../api/workbookchartaxis-delete-majorgridlines.md)|None|Delete a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Update majorGridlines](../api/workbookchartaxis-update-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Update the properties of a majorGridlines object.|
|[Get majorGridlines](../api/workbookchartaxis-get-workbookchartgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read the properties and relationships of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[List minorGridlines](../api/workbookchartaxis-list-minorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md) collection|Get the workbookChartGridlines from the minorGridlines navigation property.|
|[Create minorGridlines](../api/workbookchartaxis-post-minorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Create a new minorGridlines object.|
|[Delete minorGridlines](../api/workbookchartaxis-delete-minorgridlines.md)|None|Delete a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Update minorGridlines](../api/workbookchartaxis-update-minorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Update the properties of a minorGridlines object.|
|[Get minorGridlines](../api/workbookchartaxis-get-workbookchartgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read the properties and relationships of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[List title](../api/workbookchartaxis-list-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md) collection|Get the workbookChartAxisTitles from the title navigation property.|
|[Create title](../api/workbookchartaxis-post-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Create a new title object.|
|[Delete title](../api/workbookchartaxis-delete-title.md)|None|Delete a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|
|[Update title](../api/workbookchartaxis-update-title.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Update the properties of a title object.|
|[Get title](../api/workbookchartaxis-get-workbookchartaxistitle.md)|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|Read the properties and relationships of a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|majorUnit|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|maximum|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|minimum|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|minorUnit|[Json](../resources/intune-json.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartAxisFormat](../resources/workbookchartaxisformat.md)|**TODO: Add Description**|
|majorGridlines|[workbookChartGridlines](../resources/workbookchartgridlines.md)|**TODO: Add Description**|
|minorGridlines|[workbookChartGridlines](../resources/workbookchartgridlines.md)|**TODO: Add Description**|
|title|[workbookChartAxisTitle](../resources/workbookchartaxistitle.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxis",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "id": "String (identifier)",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

