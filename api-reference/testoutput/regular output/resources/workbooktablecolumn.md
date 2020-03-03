---
title: "workbookTableColumn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookTableColumn resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookTableColumns](../api/workbooktablecolumn-list.md)|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|List properties and relationships of the [workbookTableColumn](../resources/workbooktablecolumn.md) objects.|
|[Get workbookTableColumn](../api/workbooktablecolumn-get.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Read properties and relationships of the [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Create workbookTableColumn](../api/workbooktablecolumn-create.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Create a new [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Delete workbookTableColumn](../api/workbooktablecolumn-delete.md)|None|Deletes a [workbookTableColumn](../resources/workbooktablecolumn.md).|
|[Update workbookTableColumn](../api/workbooktablecolumn-update.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Update the properties of a [workbookTableColumn](../resources/workbooktablecolumn.md) object.|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookfilter.md)|Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|name|String||
|values|[Json](../resources/json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filter|[workbookFilter](../resources/workbookfilter.md)||

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

