---
title: "workbookFilter resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookFilter resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookFilters](../api/workbookfilter-list.md)|[workbookFilter](../resources/workbookFilter.md) collection|List properties and relationships of the [workbookFilter](../resources/workbookfilter.md) objects.|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookFilter.md)|Read properties and relationships of the [workbookFilter](../resources/workbookfilter.md) object.|
|[Create workbookFilter](../api/workbookfilter-create.md)|[workbookFilter](../resources/workbookFilter.md)|Create a new [workbookFilter](../resources/workbookfilter.md) object.|
|[Delete workbookFilter](../api/workbookfilter-delete.md)|None|Deletes a [workbookFilter](../resources/workbookfilter.md).|
|[Update workbookFilter](../api/workbookfilter-update.md)|[workbookFilter](../resources/workbookFilter.md)|Update the properties of a [workbookFilter](../resources/workbookfilter.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|criteria|[workbookFilterCriteria](../resources/workbookFilterCriteria.md)||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookFilter",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilter",
  "id": "String (identifier)",
  "criteria": {
    "@odata.type": "microsoft.graph.workbookFilterCriteria"
  }
}
```

