---
title: "workbookChartGridlines resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartGridlines resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartGridlineses](../api/workbookchartgridlines-list.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md) collection|List properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) objects.|
|[Get workbookChartGridlines](../api/workbookchartgridlines-get.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md)|Read properties and relationships of the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Create workbookChartGridlines](../api/workbookchartgridlines-create.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md)|Create a new [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Delete workbookChartGridlines](../api/workbookchartgridlines-delete.md)|None|Deletes a [workbookChartGridlines](../resources/workbookchartgridlines.md).|
|[Update workbookChartGridlines](../api/workbookchartgridlines-update.md)|[workbookChartGridlines](../resources/workbookChartGridlines.md)|Update the properties of a [workbookChartGridlines](../resources/workbookchartgridlines.md) object.|
|[Get workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-get.md)|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md)|Read properties and relationships of the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|visible|Boolean||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md)||

## JSON Representation
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

