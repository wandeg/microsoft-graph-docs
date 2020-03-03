---
title: "workbookTable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookTable resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTable](../api/workbooktable-get.md)|[workbookTable](../resources/workbookTable.md)|Read properties and relationships of the [workbookTable](../resources/workbooktable.md) object.|
|[Delete workbookTable](../api/workbooktable-delete.md)|None|Deletes a [workbookTable](../resources/workbooktable.md).|
|[Update workbookTable](../api/workbooktable-update.md)|[workbookTable](../resources/workbookTable.md)|Update the properties of a [workbookTable](../resources/workbooktable.md) object.|
|[List columns](../api/workbooktable-list-columns.md)|[workbookTableColumn](../resources/workbookTableColumn.md) collection|Get the workbookTableColumns from the columns navigation property.|
|[Add columns](../api/workbooktable-post-columns.md)|[workbookTableColumn](../resources/workbookTableColumn.md)|Add columns by posting to the columns collection.|
|[List rows](../api/workbooktable-list-rows.md)|[workbookTableRow](../resources/workbookTableRow.md) collection|Get the workbookTableRows from the rows navigation property.|
|[Add rows](../api/workbooktable-post-rows.md)|[workbookTableRow](../resources/workbookTableRow.md)|Add rows by posting to the rows collection.|
|[Get workbookTableSort](../api/workbooktablesort-get.md)|[workbookTableSort](../resources/workbookTableSort.md)|Read properties and relationships of the [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookWorksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|highlightFirstColumn|Boolean||
|highlightLastColumn|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|legacyId|String||
|name|String||
|showBandedColumns|Boolean||
|showBandedRows|Boolean||
|showFilterButton|Boolean||
|showHeaders|Boolean||
|showTotals|Boolean||
|style|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columns|[workbookTableColumn](../resources/workbookTableColumn.md) collection||
|rows|[workbookTableRow](../resources/workbookTableRow.md) collection||
|sort|[workbookTableSort](../resources/workbookTableSort.md)||
|worksheet|[workbookWorksheet](../resources/workbookWorksheet.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTable",
  "id": "String (identifier)",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String"
}
```

