---
title: "workbookTableSort resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookTableSort resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookTableSorts](../api/workbooktablesort-list.md)|[workbookTableSort](../resources/workbookTableSort.md) collection|List properties and relationships of the [workbookTableSort](../resources/workbooktablesort.md) objects.|
|[Get workbookTableSort](../api/workbooktablesort-get.md)|[workbookTableSort](../resources/workbookTableSort.md)|Read properties and relationships of the [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Create workbookTableSort](../api/workbooktablesort-create.md)|[workbookTableSort](../resources/workbookTableSort.md)|Create a new [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Delete workbookTableSort](../api/workbooktablesort-delete.md)|None|Deletes a [workbookTableSort](../resources/workbooktablesort.md).|
|[Update workbookTableSort](../api/workbooktablesort-update.md)|[workbookTableSort](../resources/workbookTableSort.md)|Update the properties of a [workbookTableSort](../resources/workbooktablesort.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fields|[workbookSortField](../resources/workbookSortField.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|matchCase|Boolean||
|method|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableSort",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "id": "String (identifier)",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField"
    }
  ],
  "matchCase": true,
  "method": "String"
}
```

