---
title: "workbookTableSort resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookTableSort resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTableSort](../api/workbooktablesort-get.md)|[workbookTableSort](../resources/workbooktablesort.md)|Read the properties and relationships of a [workbookTableSort](../resources/workbooktablesort.md) object.|
|[Update workbookTableSort](../api/workbooktablesort-update.md)|[workbookTableSort](../resources/workbooktablesort.md)|Update the properties of a [workbookTableSort](../resources/workbooktablesort.md) object.|
|[apply](../api/workbooktablesort-apply.md)|None|**TODO: Add Description**|
|[clear](../api/workbooktablesort-clear.md)|None|**TODO: Add Description**|
|[reapply](../api/workbooktablesort-reapply.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|fields|[workbookSortField](../resources/workbooksortfield.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|matchCase|Boolean|**TODO: Add Description**|
|method|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

