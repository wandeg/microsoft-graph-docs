---
title: "workbook resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbook resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbooks](../api/workbook-list.md)|[workbook](../resources/workbook.md) collection|List properties and relationships of the [workbook](../resources/workbook.md) objects.|
|[Get workbook](../api/workbook-get.md)|[workbook](../resources/workbook.md)|Read properties and relationships of the [workbook](../resources/workbook.md) object.|
|[Create workbook](../api/workbook-create.md)|[workbook](../resources/workbook.md)|Create a new [workbook](../resources/workbook.md) object.|
|[Delete workbook](../api/workbook-delete.md)|None|Deletes a [workbook](../resources/workbook.md).|
|[Update workbook](../api/workbook-update.md)|[workbook](../resources/workbook.md)|Update the properties of a [workbook](../resources/workbook.md) object.|
|[Get workbookApplication](../api/workbookapplication-get.md)|[workbookApplication](../resources/workbookApplication.md)|Read properties and relationships of the [workbookApplication](../resources/workbookapplication.md) object.|
|[List names](../api/workbook-list-names.md)|[workbookNamedItem](../resources/workbookNamedItem.md) collection|Get the workbookNamedItems from the names navigation property.|
|[Add names](../api/workbook-post-names.md)|[workbookNamedItem](../resources/workbookNamedItem.md)|Add names by posting to the names collection.|
|[List tables](../api/workbook-list-tables.md)|[workbookTable](../resources/workbookTable.md) collection|Get the workbookTables from the tables navigation property.|
|[Add tables](../api/workbook-post-tables.md)|[workbookTable](../resources/workbookTable.md)|Add tables by posting to the tables collection.|
|[List worksheets](../api/workbook-list-worksheets.md)|[workbookWorksheet](../resources/workbookWorksheet.md) collection|Get the workbookWorksheets from the worksheets navigation property.|
|[Add worksheets](../api/workbook-post-worksheets.md)|[workbookWorksheet](../resources/workbookWorksheet.md)|Add worksheets by posting to the worksheets collection.|
|[List comments](../api/workbook-list-comments.md)|[workbookComment](../resources/workbookComment.md) collection|Get the workbookComments from the comments navigation property.|
|[Add comments](../api/workbook-post-comments.md)|[workbookComment](../resources/workbookComment.md)|Add comments by posting to the comments collection.|
|[Get workbookFunctions](../api/workbookfunctions-get.md)|[workbookFunctions](../resources/workbookFunctions.md)|Read properties and relationships of the [workbookFunctions](../resources/workbookfunctions.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|application|[workbookApplication](../resources/workbookApplication.md)||
|comments|[workbookComment](../resources/workbookComment.md) collection||
|functions|[workbookFunctions](../resources/workbookFunctions.md)||
|names|[workbookNamedItem](../resources/workbookNamedItem.md) collection||
|tables|[workbookTable](../resources/workbookTable.md) collection||
|worksheets|[workbookWorksheet](../resources/workbookWorksheet.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbook",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbook",
  "id": "String (identifier)"
}
```

