---
title: "workbookRange resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookRange resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRanges](../api/workbookrange-list.md)|[workbookRange](../resources/workbookRange.md) collection|List properties and relationships of the [workbookRange](../resources/workbookrange.md) objects.|
|[Get workbookRange](../api/workbookrange-get.md)|[workbookRange](../resources/workbookRange.md)|Read properties and relationships of the [workbookRange](../resources/workbookrange.md) object.|
|[Create workbookRange](../api/workbookrange-create.md)|[workbookRange](../resources/workbookRange.md)|Create a new [workbookRange](../resources/workbookrange.md) object.|
|[Delete workbookRange](../api/workbookrange-delete.md)|None|Deletes a [workbookRange](../resources/workbookrange.md).|
|[Update workbookRange](../api/workbookrange-update.md)|[workbookRange](../resources/workbookRange.md)|Update the properties of a [workbookRange](../resources/workbookrange.md) object.|
|[Get workbookRangeFormat](../api/workbookrangeformat-get.md)|[workbookRangeFormat](../resources/workbookRangeFormat.md)|Read properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.|
|[Get workbookRangeSort](../api/workbookrangesort-get.md)|[workbookRangeSort](../resources/workbookRangeSort.md)|Read properties and relationships of the [workbookRangeSort](../resources/workbookrangesort.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookWorksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String||
|addressLocal|String||
|cellCount|Int32||
|columnCount|Int32||
|columnHidden|Boolean||
|columnIndex|Int32||
|formulas|[Json](../resources/Json.md)||
|formulasLocal|[Json](../resources/Json.md)||
|formulasR1C1|[Json](../resources/Json.md)||
|hidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|numberFormat|[Json](../resources/Json.md)||
|rowCount|Int32||
|rowHidden|Boolean||
|rowIndex|Int32||
|text|[Json](../resources/Json.md)||
|values|[Json](../resources/Json.md)||
|valueTypes|[Json](../resources/Json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|format|[workbookRangeFormat](../resources/workbookRangeFormat.md)||
|sort|[workbookRangeSort](../resources/workbookRangeSort.md)||
|worksheet|[workbookWorksheet](../resources/workbookWorksheet.md)||

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

