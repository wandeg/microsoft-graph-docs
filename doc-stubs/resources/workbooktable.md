---
title: "workbookTable resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookTable resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[clearFilters](../api/workbooktable-clearfilters.md)|None|**TODO: Add Description**|
|[convertToRange](../api/workbooktable-converttorange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[dataBodyRange](../api/workbooktable-databodyrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[headerRowRange](../api/workbooktable-headerrowrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[range](../api/workbooktable-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[totalRowRange](../api/workbooktable-totalrowrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[reapplyFilters](../api/workbooktable-reapplyfilters.md)|None|**TODO: Add Description**|
|[add](../api/workbooktable-add.md)|[workbookTable](../resources/workbooktable.md)|**TODO: Add Description**|
|[itemAt](../api/workbooktable-itemat.md)|[workbookTable](../resources/workbooktable.md)|**TODO: Add Description**|
|[count](../api/workbooktable-count.md)|Int32|**TODO: Add Description**|
|[List columns](../api/workbooktable-list-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|Get the workbookTableColumns from the columns navigation property.|
|[Create columns](../api/workbooktable-post-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Create a new columns object.|
|[Delete columns](../api/workbooktable-delete-columns.md)|None|Delete a [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Update columns](../api/workbooktable-update-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Update the properties of a columns object.|
|[Get workbookTableColumn](../api/workbooktablecolumn-get.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Read the properties and relationships of a [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[List rows](../api/workbooktable-list-rows.md)|[workbookTableRow](../resources/workbooktablerow.md) collection|Get the workbookTableRows from the rows navigation property.|
|[Create rows](../api/workbooktable-post-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Create a new rows object.|
|[Delete rows](../api/workbooktable-delete-rows.md)|None|Delete a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Update rows](../api/workbooktable-update-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Update the properties of a rows object.|
|[Get workbookTableRow](../api/workbooktablerow-get.md)|[workbookTableRow](../resources/workbooktablerow.md)|Read the properties and relationships of a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[List sort](../api/workbooktable-list-sort.md)|[workbookTableSort](../resources/workbooktablesort.md) collection|Get the workbookTableSorts from the sort navigation property.|
|[Create sort](../api/workbooktable-post-sort.md)|[workbookTableSort](../resources/workbooktablesort.md)|Create a new sort object.|
|[Delete sort](../api/workbooktable-delete-sort.md)|None|Delete a [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Update sort](../api/workbooktable-update-sort.md)|[workbookTableSort](../resources/workbooktablesort.md)|Update the properties of a sort object.|
|[Get workbookTableSort](../api/workbooktablesort-get.md)|[workbookTableSort](../resources/workbooktablesort.md)|Read the properties and relationships of a [workbookTableSort](../resources/workbooktablesort.md) object.|
|[List worksheet](../api/workbooktable-list-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|Get the workbookWorksheets from the worksheet navigation property.|
|[Create worksheet](../api/workbooktable-post-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Create a new worksheet object.|
|[Delete worksheet](../api/workbooktable-delete-worksheet.md)|None|Delete a [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[Update worksheet](../api/workbooktable-update-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Update the properties of a worksheet object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read the properties and relationships of a [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|highlightFirstColumn|Boolean|**TODO: Add Description**|
|highlightLastColumn|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|legacyId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|showBandedColumns|Boolean|**TODO: Add Description**|
|showBandedRows|Boolean|**TODO: Add Description**|
|showFilterButton|Boolean|**TODO: Add Description**|
|showHeaders|Boolean|**TODO: Add Description**|
|showTotals|Boolean|**TODO: Add Description**|
|style|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|columns|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|**TODO: Add Description**|
|rows|[workbookTableRow](../resources/workbooktablerow.md) collection|**TODO: Add Description**|
|sort|[workbookTableSort](../resources/workbooktablesort.md)|**TODO: Add Description**|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "highlightFirstColumn": "Boolean",
  "highlightLastColumn": "Boolean",
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": "Boolean",
  "showBandedRows": "Boolean",
  "showFilterButton": "Boolean",
  "showHeaders": "Boolean",
  "showTotals": "Boolean",
  "style": "String"
}
```

