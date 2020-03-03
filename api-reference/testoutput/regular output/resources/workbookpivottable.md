---
title: "workbookPivotTable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookPivotTable resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookPivotTables](../api/workbookpivottable-list.md)|[workbookPivotTable](../resources/workbookpivottable.md) collection|List properties and relationships of the [workbookPivotTable](../resources/workbookpivottable.md) objects.|
|[Get workbookPivotTable](../api/workbookpivottable-get.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Read properties and relationships of the [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Create workbookPivotTable](../api/workbookpivottable-create.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Create a new [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Delete workbookPivotTable](../api/workbookpivottable-delete.md)|None|Deletes a [workbookPivotTable](../resources/workbookpivottable.md).|
|[Update workbookPivotTable](../api/workbookpivottable-update.md)|[workbookPivotTable](../resources/workbookpivottable.md)|Update the properties of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookworksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookworksheet.md)||

## JSON Representation
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

