---
title: "plannerAssignedToTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerAssignedToTaskBoardTaskFormat resource type




Inherits from [plannerDelta](../resources/plannerDelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerAssignedToTaskBoardTaskFormats](../api/plannerassignedtotaskboardtaskformat-list.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md) collection|List properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) objects.|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Create plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-create.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md)|Create a new [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Delete plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-delete.md)|None|Deletes a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md).|
|[Update plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-update.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md)|Update the properties of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](../resources/plannerOrderHintsByAssignee.md)||
|unassignedOrderHint|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "id": "String (identifier)",
  "unassignedOrderHint": "String",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
}
```

