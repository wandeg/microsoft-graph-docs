---
title: "workbookRange resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookRange resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRanges](../api/workbookrange-list.md)|[workbookRange](../resources/workbookrange.md) collection|List properties and relationships of the [workbookRange](../resources/workbookrange.md) objects.|
|[Get workbookRange](../api/workbookrange-get.md)|[workbookRange](../resources/workbookrange.md)|Read properties and relationships of the [workbookRange](../resources/workbookrange.md) object.|
|[Create workbookRange](../api/workbookrange-create.md)|[workbookRange](../resources/workbookrange.md)|Create a new [workbookRange](../resources/workbookrange.md) object.|
|[Delete workbookRange](../api/workbookrange-delete.md)|None|Deletes a [workbookRange](../resources/workbookrange.md).|
|[Update workbookRange](../api/workbookrange-update.md)|[workbookRange](../resources/workbookrange.md)|Update the properties of a [workbookRange](../resources/workbookrange.md) object.|
|[clear](../api/workbookrange-clear.md)|None||
|[delete](../api/workbookrange-delete.md)|None||
|[boundingRect](../api/workbookrange-boundingrect.md)|[workbookRange](../resources/workbookrange.md)||
|[cell](../api/workbookrange-cell.md)|[workbookRange](../resources/workbookrange.md)||
|[column](../api/workbookrange-column.md)|[workbookRange](../resources/workbookrange.md)||
|[columnsAfter](../api/workbookrange-columnsafter.md)|[workbookRange](../resources/workbookrange.md)||
|[columnsAfter](../api/workbookrange-columnsafter.md)|[workbookRange](../resources/workbookrange.md)||
|[columnsBefore](../api/workbookrange-columnsbefore.md)|[workbookRange](../resources/workbookrange.md)||
|[columnsBefore](../api/workbookrange-columnsbefore.md)|[workbookRange](../resources/workbookrange.md)||
|[entireColumn](../api/workbookrange-entirecolumn.md)|[workbookRange](../resources/workbookrange.md)||
|[entireRow](../api/workbookrange-entirerow.md)|[workbookRange](../resources/workbookrange.md)||
|[intersection](../api/workbookrange-intersection.md)|[workbookRange](../resources/workbookrange.md)||
|[lastCell](../api/workbookrange-lastcell.md)|[workbookRange](../resources/workbookrange.md)||
|[lastColumn](../api/workbookrange-lastcolumn.md)|[workbookRange](../resources/workbookrange.md)||
|[lastRow](../api/workbookrange-lastrow.md)|[workbookRange](../resources/workbookrange.md)||
|[offsetRange](../api/workbookrange-offsetrange.md)|[workbookRange](../resources/workbookrange.md)||
|[resizedRange](../api/workbookrange-resizedrange.md)|[workbookRange](../resources/workbookrange.md)||
|[row](../api/workbookrange-row.md)|[workbookRange](../resources/workbookrange.md)||
|[rowsAbove](../api/workbookrange-rowsabove.md)|[workbookRange](../resources/workbookrange.md)||
|[rowsAbove](../api/workbookrange-rowsabove.md)|[workbookRange](../resources/workbookrange.md)||
|[rowsBelow](../api/workbookrange-rowsbelow.md)|[workbookRange](../resources/workbookrange.md)||
|[rowsBelow](../api/workbookrange-rowsbelow.md)|[workbookRange](../resources/workbookrange.md)||
|[usedRange](../api/workbookrange-usedrange.md)|[workbookRange](../resources/workbookrange.md)||
|[usedRange](../api/workbookrange-usedrange.md)|[workbookRange](../resources/workbookrange.md)||
|[visibleView](../api/workbookrange-visibleview.md)|[workbookRangeView](../resources/workbookrangeview.md)||
|[insert](../api/workbookrange-insert.md)|[workbookRange](../resources/workbookrange.md)||
|[merge](../api/workbookrange-merge.md)|None||
|[unmerge](../api/workbookrange-unmerge.md)|None||
|[Get workbookRangeFormat](../api/workbookrangeformat-get.md)|[workbookRangeFormat](../resources/workbookrangeformat.md)|Read properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Get workbookRangeSort](../api/workbookrangesort-get.md)|[workbookRangeSort](../resources/workbookrangesort.md)|Read properties and relationships of the [workbookRangeSort](../resources/workbookrangesort.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String||
|addressLocal|String||
|cellCount|Int32||
|columnCount|Int32||
|columnHidden|Boolean||
|columnIndex|Int32||
|formulas|[Json](../resources/json.md)||
|formulasLocal|[Json](../resources/json.md)||
|formulasR1C1|[Json](../resources/json.md)||
|hidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|numberFormat|[Json](../resources/json.md)||
|rowCount|Int32||
|rowHidden|Boolean||
|rowIndex|Int32||
|text|[Json](../resources/json.md)||
|values|[Json](../resources/json.md)||
|valueTypes|[Json](../resources/json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookRangeFormat](../resources/workbookrangeformat.md)||
|sort|[workbookRangeSort](../resources/workbookrangesort.md)||
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRange",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRange",
  "id": "String (identifier)",
  "address": "String",
  "addressLocal": "String",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "hidden": true,
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": {
    "@odata.type": "microsoft.graph.Json"
  },
  "valueTypes": {
    "@odata.type": "microsoft.graph.Json"
  },
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

