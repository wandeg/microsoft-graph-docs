---
title: "workbookWorksheet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookWorksheet resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookWorksheets](../api/workbookworksheet-list.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|List properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) objects.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[Create workbookWorksheet](../api/workbookworksheet-create.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Create a new [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[Delete workbookWorksheet](../api/workbookworksheet-delete.md)|None|Deletes a [workbookWorksheet](../resources/workbookworksheet.md).|
|[Update workbookWorksheet](../api/workbookworksheet-update.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Update the properties of a [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[List charts](../api/workbookworksheet-list-charts.md)|[workbookChart](../resources/workbookchart.md) collection|Get the workbookCharts from the charts navigation property.|
|[Add charts](../api/workbookworksheet-post-charts.md)|[workbookChart](../resources/workbookchart.md)|Add charts by posting to the charts collection.|
|[List names](../api/workbookworksheet-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Add names](../api/workbookworksheet-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Add names by posting to the names collection.|
|[List pivotTables](../api/workbookworksheet-list-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|Get the workbookPivotTables from the pivotTables navigation property.|
|[Add pivotTables](../api/workbookworksheet-post-pivottables.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Add pivotTables by posting to the pivotTables collection.|
|[Get workbookWorksheetProtection](../api/workbookworksheetprotection-get.md)|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)|Read properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.|
|[List tables](../api/workbookworksheet-list-tables.md)|[workbookTable](../resources/workbooktable.md) collection|Get the workbookTables from the tables navigation property.|
|[Add tables](../api/workbookworksheet-post-tables.md)|[workbookTable](../resources/workbooktable.md)|Add tables by posting to the tables collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|position|Int32||
|visibility|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|charts|[workbookChart](../resources/workbookchart.md) collection||
|names|[workbookNamedItem](../resources/workbooknameditem.md) collection||
|pivotTables|[workbookPivotTable](../resources/workbookpivottable.md) collection||
|protection|[workbookWorksheetProtection](../resources/workbookworksheetprotection.md)||
|tables|[workbookTable](../resources/workbooktable.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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
  "position": 1024,
  "visibility": "String"
}
```

