---
title: "workbookChartGridlines resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookChartGridlines resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Read properties and relationships of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Update workbookChartGridlines](../api/workbookchartgridlines-update.md)|[workbookChartGridlines](../resources/workbookchartgridlines.md)|Update the properties of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[List format](../api/workbookchartgridlines-list-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) collection|Get the workbookChartGridlinesFormats from the format navigation property.|
|[Create format](../api/workbookchartgridlines-post-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartgridlines-delete-format.md)|None|Delete a format object.|
|[Update format](../api/workbookchartgridlines-update-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Update the properties of a format object.|
|[Get workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-get.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Read properties and relationships of a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|

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
Here is a JSON representation of the resource.
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
  "visible": true
}
```

