---
title: "workbookChartPoint resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartPoint resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[itemAt](../api/workbookchartpoint-itemat.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|**TODO: Add Description**|
|[count](../api/workbookchartpoint-count.md)|Int32|**TODO: Add Description**|
|[List format](../api/workbookchartpoint-list-format.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md) collection|Get the workbookChartPointFormats from the format navigation property.|
|[Create format](../api/workbookchartpoint-post-format.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Create a new format object.|
|[Delete format](../api/workbookchartpoint-delete-format.md)|None|Delete a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[Update format](../api/workbookchartpoint-update-format.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Update the properties of a format object.|
|[Get workbookChartPointFormat](../api/workbookchartpointformat-get.md)|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|Read the properties and relationships of a [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.|
|[List points](../api/workbookchartseries-list-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md) collection|Get the workbookChartPoints from the points navigation property.|
|[Create points](../api/workbookchartseries-post-points.md)|[workbookChartPoint](../resources/workbookchartpoint.md)|Create a new points object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|value|[Json](../resources/json.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookChartPointFormat](../resources/workbookchartpointformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "id": "String (identifier)",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

