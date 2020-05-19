---
title: "workbookNamedItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookNamedItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List names](../api/workbook-list-names.md)|[workbookNamedItem](../resources/workbooknameditem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Create names](../api/workbook-post-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Create a new names object.|
|[Delete names](../api/workbook-delete-names.md)|None|Delete a [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[Update names](../api/workbook-update-names.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Update the properties of a names object.|
|[Get names](../api/workbook-get-workbooknameditem.md)|[workbookNamedItem](../resources/workbooknameditem.md)|Read the properties and relationships of a [workbookNamedItem](../resources/workbooknameditem.md) object.|
|[range](../api/workbooknameditem-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[add](../api/workbooknameditem-add.md)|[workbookNamedItem](../resources/workbooknameditem.md)|**TODO: Add Description**|
|[addFormulaLocal](../api/workbooknameditem-addformulalocal.md)|[workbookNamedItem](../resources/workbooknameditem.md)|**TODO: Add Description**|
|[List worksheet](../api/workbooknameditem-list-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md) collection|Get the workbookWorksheets from the worksheet navigation property.|
|[Create worksheet](../api/workbooknameditem-post-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Create a new worksheet object.|
|[Delete worksheet](../api/workbooknameditem-delete-worksheet.md)|None|Delete a [workbookWorksheet](../resources/workbookworksheet.md) object.|
|[Update worksheet](../api/workbooknameditem-update-worksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Update the properties of a worksheet object.|
|[Get worksheet](../api/workbooknameditem-get-workbookworksheet.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read the properties and relationships of a [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|comment|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|scope|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|value|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "id": "String (identifier)",
  "comment": "String",
  "name": "String",
  "scope": "String",
  "type": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": "Boolean"
}
```

