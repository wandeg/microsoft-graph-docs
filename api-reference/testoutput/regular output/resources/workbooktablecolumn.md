---
title: "workbookTableColumn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookTableColumn resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTableColumn](../api/workbooktablecolumn-get.md)|[workbookTableColumn](../resources/workbookTableColumn.md)|Read properties and relationships of the [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Delete workbookTableColumn](../api/workbooktablecolumn-delete.md)|None|Deletes a [workbookTableColumn](../resources/workbooktablecolumn.md).|
|[Update workbookTableColumn](../api/workbooktablecolumn-update.md)|[workbookTableColumn](../resources/workbookTableColumn.md)|Update the properties of a [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookFilter.md)|Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|name|String||
|values|[Json](../resources/Json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filter|[workbookFilter](../resources/workbookFilter.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "id": "String (identifier)",
  "index": 1024,
  "name": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

