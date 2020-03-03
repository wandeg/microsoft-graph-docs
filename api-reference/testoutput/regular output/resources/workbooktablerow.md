---
title: "workbookTableRow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookTableRow resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookTableRows](../api/workbooktablerow-list.md)|[workbookTableRow](../resources/workbooktablerow.md) collection|List properties and relationships of the [workbookTableRow](../resources/workbooktablerow.md) objects.|
|[Get workbookTableRow](../api/workbooktablerow-get.md)|[workbookTableRow](../resources/workbooktablerow.md)|Read properties and relationships of the [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Create workbookTableRow](../api/workbooktablerow-create.md)|[workbookTableRow](../resources/workbooktablerow.md)|Create a new [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Delete workbookTableRow](../api/workbooktablerow-delete.md)|None|Deletes a [workbookTableRow](../resources/workbooktablerow.md).|
|[Update workbookTableRow](../api/workbooktablerow-update.md)|[workbookTableRow](../resources/workbooktablerow.md)|Update the properties of a [workbookTableRow](../resources/workbooktablerow.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|values|[Json](../resources/json.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "id": "String (identifier)",
  "index": 1024,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

