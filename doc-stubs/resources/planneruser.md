---
title: "plannerUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List planner](../api/user-list-planner.md)|[plannerUser](../resources/planneruser.md) collection|Get the plannerUsers from the planner navigation property.|
|[Create planner](../api/user-post-planner.md)|[plannerUser](../resources/planneruser.md)|Create a new planner object.|
|[Delete planner](../api/user-delete-planner.md)|None|Delete a [plannerUser](../resources/planneruser.md) object.|
|[Update planner](../api/user-update-planner.md)|[plannerUser](../resources/planneruser.md)|Update the properties of a planner object.|
|[Get planner](../api/user-get-planneruser.md)|[plannerUser](../resources/planneruser.md)|Read the properties and relationships of a [plannerUser](../resources/planneruser.md) object.|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[Remove tasks](../api/planneruser-delete-tasks.md)|None|Remove a [plannerTask](../resources/plannertask.md) object.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Add plans](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|
|[Remove plans](../api/planneruser-delete-plans.md)|None|Remove a [plannerPlan](../resources/plannerplan.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|plans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "String (identifier)"
}
```

