---
title: "plannerPlan resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerPlan resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [plannerDelta](../resources/plannerdelta.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tasks](../api/plannerplan-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/plannerplan-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[Remove tasks](../api/plannerplan-delete-tasks.md)|None|Remove a [plannerTask](../resources/plannertask.md) object.|
|[List buckets](../api/plannerplan-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Add buckets](../api/plannerplan-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Add buckets by posting to the buckets collection.|
|[Remove buckets](../api/plannerplan-delete-buckets.md)|None|Remove a [plannerBucket](../resources/plannerbucket.md) object.|
|[List details](../api/plannerplan-list-details.md)|[plannerPlanDetails](../resources/plannerplandetails.md) collection|Get the plannerPlanDetails from the details navigation property.|
|[Create details](../api/plannerplan-post-details.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Create a new details object.|
|[Delete details](../api/plannerplan-delete-details.md)|None|Delete a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Update details](../api/plannerplan-update-details.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Update the properties of a details object.|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Read the properties and relationships of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[List plans](../api/plannergroup-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Add plans](../api/plannergroup-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contexts|[plannerPlanContextCollection](../resources/plannerplancontextcollection.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|owner|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|buckets|[plannerBucket](../resources/plannerbucket.md) collection|**TODO: Add Description**|
|details|[plannerPlanDetails](../resources/plannerplandetails.md)|**TODO: Add Description**|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlan",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "owner": "String",
  "title": "String",
  "contexts": {
    "@odata.type": "microsoft.graph.plannerPlanContextCollection"
  }
}
```

