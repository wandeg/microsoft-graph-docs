---
title: "plannerPlan resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerPlan resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerPlan](../api/plannerplan-get.md)|[plannerPlan](../resources/plannerPlan.md)|Read properties and relationships of the [plannerPlan](../resources/plannerplan.md) object.|
|[Delete plannerPlan](../api/plannerplan-delete.md)|None|Deletes a [plannerPlan](../resources/plannerplan.md).|
|[Update plannerPlan](../api/plannerplan-update.md)|[plannerPlan](../resources/plannerPlan.md)|Update the properties of a [plannerPlan](../resources/plannerplan.md) object.|
|[List tasks](../api/plannerplan-list-tasks.md)|[plannerTask](../resources/plannerTask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/plannerplan-post-tasks.md)|[plannerTask](../resources/plannerTask.md)|Create tasks by posting to the tasks collection.|
|[List buckets](../api/plannerplan-list-buckets.md)|[plannerBucket](../resources/plannerBucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Create buckets](../api/plannerplan-post-buckets.md)|[plannerBucket](../resources/plannerBucket.md)|Create buckets by posting to the buckets collection.|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerPlanDetails.md)|Read properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|owner|String||
|title|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|buckets|[plannerBucket](../resources/plannerBucket.md) collection||
|details|[plannerPlanDetails](../resources/plannerPlanDetails.md)||
|tasks|[plannerTask](../resources/plannerTask.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlan",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "String (timestamp)",
  "owner": "String",
  "title": "String"
}
```

