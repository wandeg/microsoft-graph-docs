---
title: "workbookPivotTable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookPivotTable resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookPivotTable](../api/workbookpivottable-get.md)|[workbookPivotTable](../resources/workbookPivotTable.md)|Read properties and relationships of the [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Delete workbookPivotTable](../api/workbookpivottable-delete.md)|None|Deletes a [workbookPivotTable](../resources/workbookpivottable.md).|
|[Update workbookPivotTable](../api/workbookpivottable-update.md)|[workbookPivotTable](../resources/workbookPivotTable.md)|Update the properties of a [workbookPivotTable](../resources/workbookpivottable.md) object.|
|[Get workbookWorksheet](../api/workbookworksheet-get.md)|[workbookWorksheet](../resources/workbookWorksheet.md)|Read properties and relationships of the [workbookWorksheet](../resources/workbookworksheet.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|worksheet|[workbookWorksheet](../resources/workbookWorksheet.md)||

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

