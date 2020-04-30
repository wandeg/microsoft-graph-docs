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


Inherits from [plannerDelta](../resources/plannerdelta.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[Remove tasks](../api/planneruser-delete-tasks.md)|None|Remove a [plannerTask](../resources/plannertask.md) object.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Add plans](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|
|[Remove plans](../api/planneruser-delete-plans.md)|None|Remove a [plannerPlan](../resources/plannerplan.md) object.|
|[List favoritePlans](../api/planneruser-list-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the favoritePlans navigation property.|
|[Add favoritePlans](../api/planneruser-post-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md)|Add favoritePlans by posting to the favoritePlans collection.|
|[Remove favoritePlans](../api/planneruser-delete-favoriteplans.md)|None|Remove a [plannerPlan](../resources/plannerplan.md) object.|
|[List recentPlans](../api/planneruser-list-recentplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the recentPlans navigation property.|
|[Add recentPlans](../api/planneruser-post-recentplans.md)|[plannerPlan](../resources/plannerplan.md)|Add recentPlans by posting to the recentPlans collection.|
|[Remove recentPlans](../api/planneruser-delete-recentplans.md)|None|Remove a [plannerPlan](../resources/plannerplan.md) object.|
|[List all](../api/planneruser-list-all.md)|[plannerDelta](../resources/plannerdelta.md) collection|Get the plannerDeltas from the all navigation property.|
|[Add all](../api/planneruser-post-all.md)|[plannerDelta](../resources/plannerdelta.md)|Add all by posting to the all collection.|
|[Remove all](../api/planneruser-delete-all.md)|None|Remove an [plannerDelta](../resources/plannerdelta.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|all|[plannerDelta](../resources/plannerdelta.md) collection|**TODO: Add Description**|
|favoritePlans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|plans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|recentPlans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

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

