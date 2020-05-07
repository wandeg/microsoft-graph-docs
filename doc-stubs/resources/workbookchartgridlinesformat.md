---
title: "workbookChartGridlinesFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartGridlinesFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List line](../api/workbookchartgridlinesformat-list-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md) collection|Get the workbookChartLineFormats from the line navigation property.|
|[Create line](../api/workbookchartgridlinesformat-post-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Create a new line object.|
|[Delete line](../api/workbookchartgridlinesformat-delete-line.md)|None|Delete a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[Update line](../api/workbookchartgridlinesformat-update-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Update the properties of a line object.|
|[Get workbookChartLineFormat](../api/workbookchartlineformat-get.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Read the properties and relationships of a [workbookChartLineFormat](../resources/workbookchartlineformat.md) object.|
|[List format](../api/workbookchartgridlines-list-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md) collection|Get the workbookChartGridlinesFormats from the format navigation property.|
|[Create format](../api/workbookchartgridlines-post-format.md)|[workbookChartGridlinesFormat](../resources/workbookchartgridlinesformat.md)|Create a new format object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|line|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

