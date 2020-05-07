---
title: "plannerBucket resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerBucket resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [plannerDelta](../resources/plannerdelta.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tasks](../api/plannerbucket-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/plannerbucket-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[Remove tasks](../api/plannerbucket-delete-tasks.md)|None|Remove a [plannerTask](../resources/plannertask.md) object.|
|[List buckets](../api/plannerplan-list-buckets.md)|[plannerBucket](../resources/plannerbucket.md) collection|Get the plannerBuckets from the buckets navigation property.|
|[Add buckets](../api/plannerplan-post-buckets.md)|[plannerBucket](../resources/plannerbucket.md)|Add buckets by posting to the buckets collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerBucket",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "String (identifier)",
  "name": "String",
  "planId": "String",
  "orderHint": "String"
}
```

