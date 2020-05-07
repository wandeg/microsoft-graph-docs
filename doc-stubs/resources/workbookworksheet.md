---
title: "workbookWorksheet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookWorksheet resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[cell](../api/workbookworksheet-cell.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[range](../api/workbookworksheet-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[range](../api/workbookworksheet-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[usedRange](../api/workbookworksheet-usedrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[usedRange](../api/workbookworksheet-usedrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[add](../api/workbookworksheet-add.md)|[workbookWorksheet](../resources/workbookworksheet.md)|**TODO: Add Description**|
|[List charts](../api/workbookworksheet-list-charts.md)|[workbookChart](../resources/workbookchart.md) collection|Get the workbookCharts from the charts navigation property.|
|[Create charts](../api/workbookworksheet-post-charts.md)|[workbookChart](../resources/workbookchart.md)|Create a new charts object.|
|[Delete charts](../api/workbookworksheet-delete-charts.md)|None|Delete a [workbookChart](../resources/workbookchart.md) object.|
|[Update charts](../api/workbookworksheet-update-charts.md)|[workbookChart](../resources/workbookchart.md)|Update the properties of a charts object.|
|[Get workbookChart](../api/workbookchart-get.md)|[workbookChart](../resources/workbookchart.md)|Read the properties and relationships of a [workbookChart](../resources/workbookchart.md) object.|
|[List names](../api/workbookworksheet-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Create names](../api/workbookworksheet-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Create a new names object.|
|[Delete names](../api/workbookworksheet-delete-names.md)|None|Delete a [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[Update names](../api/workbookworksheet-update-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Update the properties of a names object.|
|[Get workbookNamedItem](../api/workbooknameditem-get.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Read the properties and relationships of a [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[List pivotTables](../api/workbookworksheet-list-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|Get the workbookPivotTables from the pivotTables navigation property.|
|[Create pivotTables](../api/workbookworksheet-post-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Create a new pivotTables object.|
|[Delete pivotTables](../api/workbookworksheet-delete-pivottables.md)|None|Delete a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Update pivotTables](../api/workbookworksheet-update-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Update the properties of a pivotTables object.|
|[Get workbookPivotTable](../api/workbookpivottable-get.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Read the properties and relationships of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[List protection](../api/workbookworksheet-list-protection.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md) collection|Get the workbookWorksheetProtections from the protection navigation property.|
|[Create protection](../api/workbookworksheet-post-protection.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Create a new protection object.|
|[Delete protection](../api/workbookworksheet-delete-protection.md)|None|Delete a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[Update protection](../api/workbookworksheet-update-protection.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Update the properties of a protection object.|
|[Get workbookWorksheetProtection](../api/workbookworksheetprotection-get.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Read the properties and relationships of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[List tables](../api/workbookworksheet-list-tables.md)|[workbookTable](../resources/workbooktable.md) collection|Get the workbookTables from the tables navigation property.|
|[Create tables](../api/workbookworksheet-post-tables.md)|[workbookTable](../resources/workbooktable.md)|Create a new tables object.|
|[Delete tables](../api/workbookworksheet-delete-tables.md)|None|Delete a [workbookTable](../resources/workbooktable.md) object.|
|[Update tables](../api/workbookworksheet-update-tables.md)|[workbookTable](../resources/workbooktable.md)|Update the properties of a tables object.|
|[Get workbookTable](../api/workbooktable-get.md)|[workbookTable](../resources/workbooktable.md)|Read the properties and relationships of a [workbookTable](../resources/workbooktable.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|position|Int32|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|charts|[workbookChart](../resources/workbookchart.md) collection|**TODO: Add Description**|
|names|[workbookNamedItem](../resources/workbooknameditem.md) collection|**TODO: Add Description**|
|pivotTables|[workbookPivotTable](../resources/workbookpivottable.md) collection|**TODO: Add Description**|
|protection|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|**TODO: Add Description**|
|tables|[workbookTable](../resources/workbooktable.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "String (identifier)",
  "name": "String",
  "position": "Integer",
  "visibility": "String"
}
```

