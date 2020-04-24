---
title: "plannerAssignedToTaskBoardTaskFormat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerAssignedToTaskBoardTaskFormat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [plannerDelta](../resources/plannerdelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Read the properties and relationships of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Update plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-update.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Update the properties of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](../resources/plannerorderhintsbyassignee.md)|**TODO: Add Description**|
|unassignedOrderHint|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

