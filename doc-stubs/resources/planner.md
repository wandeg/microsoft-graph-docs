---
title: "planner resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# planner resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tasks](../api/planner-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/planner-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Create a new tasks object.|
|[Delete tasks](../api/planner-delete-tasks.md)|None|Delete a [plannerTask](../resources/plannertask.md) object.|
|[Update tasks](../api/planner-update-tasks.md)|[plannerTask](../resources/plannertask.md)|Update the properties of a tasks object.|
|[Get tasks](../api/planner-get-plannertask.md)|[plannerTask](../resources/plannertask.md)|Read the properties and relationships of a [plannerTask](../resources/plannertask.md) object.|
|[List plans](../api/planner-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlans from the plans navigation property.|
|[Create plans](../api/planner-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Create a new plans object.|
|[Delete plans](../api/planner-delete-plans.md)|None|Delete a [plannerPlan](../resources/plannerplan.md) object.|
|[Update plans](../api/planner-update-plans.md)|[plannerPlan](../resources/plannerplan.md)|Update the properties of a plans object.|
|[Get plans](../api/planner-get-plannerplan.md)|[plannerPlan](../resources/plannerplan.md)|Read the properties and relationships of a [plannerPlan](../resources/plannerplan.md) object.|
|[List buckets](../api/planner-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Create buckets](../api/planner-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Create a new buckets object.|
|[Delete buckets](../api/planner-delete-buckets.md)|None|Delete a [plannerBucket](../resources/plannerbucket.md) object.|
|[Update buckets](../api/planner-update-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Update the properties of a buckets object.|
|[Get buckets](../api/planner-get-plannerbucket.md)|[plannerBucket](../resources/plannerbucket.md)|Read the properties and relationships of a [plannerBucket](../resources/plannerbucket.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|buckets|[plannerBucket](../resources/plannerbucket.md) collection|**TODO: Add Description**|
|plans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.planner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.planner",
  "id": "String (identifier)"
}
```

