---
title: "plannerUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerUser resource type


Namespace: microsoft.graph




Inherits from [plannerDelta](../resources/plannerdelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/planneruser.md)|Read properties and relationships of the [plannerUser](../resources/planneruser.md) object.|
|[Update plannerUser](../api/planneruser-update.md)|[plannerUser](../resources/planneruser.md)|Update the properties of a [plannerUser](../resources/planneruser.md) object.|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Create tasks by posting to the tasks collection.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Create plans by posting to the plans collection.|
|[List favoritePlans](../api/planneruser-list-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the favoritePlans navigation property.|
|[Create favoritePlans](../api/planneruser-post-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md)|Create favoritePlans by posting to the favoritePlans collection.|
|[List recentPlans](../api/planneruser-list-recentplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the recentPlans navigation property.|
|[Create recentPlans](../api/planneruser-post-recentplans.md)|[plannerPlan](../resources/plannerplan.md)|Create recentPlans by posting to the recentPlans collection.|
|[List all](../api/planneruser-list-all.md)|[plannerDelta](../resources/plannerdelta.md) collection|Get the plannerDeltas from the all navigation property.|
|[Create all](../api/planneruser-post-all.md)|[plannerDelta](../resources/plannerdelta.md)|Create all by posting to the all collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|all|[plannerDelta](../resources/plannerdelta.md) collection||
|favoritePlans|[plannerPlan](../resources/plannerplan.md) collection||
|plans|[plannerPlan](../resources/plannerplan.md) collection||
|recentPlans|[plannerPlan](../resources/plannerplan.md) collection||
|tasks|[plannerTask](../resources/plannertask.md) collection||

## JSON representation
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

