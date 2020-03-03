---
title: "workbookChartGridlinesFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookChartGridlinesFormat resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartGridlinesFormats](../api/workbookchartgridlinesformat-list.md)|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md) collection|List properties and relationships of the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) objects.|
|[Get workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-get.md)|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md)|Read properties and relationships of the [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|
|[Create workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-create.md)|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md)|Create a new [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|
|[Delete workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-delete.md)|None|Deletes a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md).|
|[Update workbookChartGridlinesFormat](../api/workbookchartgridlinesformat-update.md)|[workbookChartGridlinesFormat](../resources/workbookChartGridlinesFormat.md)|Update the properties of a [workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookChartLineFormat.md)|Read properties and relationships of the [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|line|[workbookChartLineFormat](../resources/workbookChartLineFormat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartGridlinesFormat",
  "id": "String (identifier)"
}
```

