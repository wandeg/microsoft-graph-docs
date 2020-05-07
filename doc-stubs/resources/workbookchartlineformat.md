---
title: "workbookChartLineFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookChartLineFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[clear](../api/workbookchartlineformat-clear.md)|None|**TODO: Add Description**|
|[List line](../api/workbookchartaxisformat-list-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md) collection|Get the workbookChartLineFormats from the line navigation property.|
|[Create line](../api/workbookchartaxisformat-post-line.md)|[workbookChartLineFormat](../resources/workbookchartlineformat.md)|Create a new line object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartLineFormat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartLineFormat",
  "id": "String (identifier)",
  "color": "String"
}
```

