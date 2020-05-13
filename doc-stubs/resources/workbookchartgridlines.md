---
title: "workbookChartGridlines resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartGridlines resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List majorGridlines](../api/workbookchartaxis-list-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md) collection|Get the workbookChartGridlines from the majorGridlines navigation property.|
|[Create majorGridlines](../api/workbookchartaxis-post-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Create a new majorGridlines object.|
|[Delete majorGridlines](../api/workbookchartaxis-delete-majorgridlines.md)|None|Delete a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Update majorGridlines](../api/workbookchartaxis-update-majorgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Update the properties of a majorGridlines object.|
|[Get majorGridlines](../api/workbookchartaxis-get-workbookchartgridlines.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read the properties and relationships of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[List format](../api/workbookchartgridlines-list-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) collection|Get the workbookChartGridlinesFormats from the format navigation property.|
|[Create format](../api/workbookchartgridlines-post-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartgridlines-delete-format.md)|None|Delete a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|
|[Update format](../api/workbookchartgridlines-update-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Update the properties of a format object.|
|[Get format](../api/workbookchartgridlines-get-workbookchartgridlinesformat.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Read the properties and relationships of a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|visible|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartGridlines",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartGridlines",
  "id": "String (identifier)",
  "visible": "Boolean"
}
```

