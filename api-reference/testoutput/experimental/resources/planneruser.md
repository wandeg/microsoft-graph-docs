---
title: "plannerUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerUser resource type




Inherits from [plannerDelta](../resources/plannerDelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerUsers](../api/planneruser-list.md)|[plannerUser](../resources/plannerUser.md) collection|List properties and relationships of the [plannerUser](../resources/planneruser.md) objects.|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/plannerUser.md)|Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.|
|[Create plannerUser](../api/planneruser-create.md)|[plannerUser](../resources/plannerUser.md)|Create a new [plannerUser](../resources/planneruser.md) object.|
|[Delete plannerUser](../api/planneruser-delete.md)|None|Deletes a [plannerUser](../resources/planneruser.md).|
|[Update plannerUser](../api/planneruser-update.md)|[plannerUser](../resources/plannerUser.md)|Update the properties of a [plannerUser](../resources/planneruser.md) object.|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannerTask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannerTask.md)|Create tasks by posting to the tasks collection.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerPlan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerPlan.md)|Create plans by posting to the plans collection.|
|[List favoritePlans](../api/planneruser-list-favoriteplans.md)|[plannerPlan](../resources/plannerPlan.md) collection|Get the plannerPlans from the favoritePlans navigation property.|
|[Create favoritePlans](../api/planneruser-post-favoriteplans.md)|[plannerPlan](../resources/plannerPlan.md)|Create favoritePlans by posting to the favoritePlans collection.|
|[List recentPlans](../api/planneruser-list-recentplans.md)|[plannerPlan](../resources/plannerPlan.md) collection|Get the plannerPlans from the recentPlans navigation property.|
|[Create recentPlans](../api/planneruser-post-recentplans.md)|[plannerPlan](../resources/plannerPlan.md)|Create recentPlans by posting to the recentPlans collection.|
|[List all](../api/planneruser-list-all.md)|[plannerDelta](../resources/plannerDelta.md) collection|Get the plannerDeltas from the all navigation property.|
|[Create all](../api/planneruser-post-all.md)|[plannerDelta](../resources/plannerDelta.md)|Create all by posting to the all collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](../resources/plannerFavoritePlanReferenceCollection.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerRecentPlanReferenceCollection.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|all|[plannerDelta](../resources/plannerDelta.md) collection||
|favoritePlans|[plannerPlan](../resources/plannerPlan.md) collection||
|plans|[plannerPlan](../resources/plannerPlan.md) collection||
|recentPlans|[plannerPlan](../resources/plannerPlan.md) collection||
|tasks|[plannerTask](../resources/plannerTask.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerUser",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "String (identifier)",
  "favoritePlanReferences": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
  },
  "recentPlanReferences": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
  }
}
```

