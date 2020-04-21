---
title: "workbookPivotTable resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookPivotTable resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookPivotTable](../api/workbookpivottable-get.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Read properties and relationships of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Update workbookPivotTable](../api/workbookpivottable-update.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Update the properties of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[refresh](../api/workbookpivottable-refresh.md)|None|**TODO: Add Description**|
|[refreshAll](../api/workbookpivottable-refreshall.md)|None|**TODO: Add Description**|
|[List worksheet](../api/workbookpivottable-list-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|Get the workbookWorksheets from the worksheet navigation property.|
|[Create worksheet](../api/workbookpivottable-post-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Create a new worksheet object.|
|[Delete worksheet](../api/workbookpivottable-delete-worksheet.md)|None|Delete a worksheet object.|
|[Update worksheet](../api/workbookpivottable-update-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Update the properties of a worksheet object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of a [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[List pivotTables](../api/workbookworksheet-list-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|Get the workbookPivotTables from the pivotTables navigation property.|
|[Create pivotTables](../api/workbookworksheet-post-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Create a new pivotTables object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookPivotTable",
  "id": "String (identifier)",
  "name": "String"
}
```

