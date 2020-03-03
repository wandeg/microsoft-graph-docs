---
title: "plannerBucket resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerBucket resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerBucket](../api/plannerbucket-get.md)|[plannerBucket](../resources/plannerBucket.md)|Read properties and relationships of the [plannerBucket](../resources/plannerbucket.md) object.|
|[Delete plannerBucket](../api/plannerbucket-delete.md)|None|Deletes a [plannerBucket](../resources/plannerbucket.md).|
|[Update plannerBucket](../api/plannerbucket-update.md)|[plannerBucket](../resources/plannerBucket.md)|Update the properties of a [plannerBucket](../resources/plannerbucket.md) object.|
|[List tasks](../api/plannerbucket-list-tasks.md)|[plannerTask](../resources/plannerTask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Create tasks](../api/plannerbucket-post-tasks.md)|[plannerTask](../resources/plannerTask.md)|Create tasks by posting to the tasks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|orderHint|String||
|planId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|tasks|[plannerTask](../resources/plannerTask.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerBucket",
  "baseType": "microsoft.graph.entity",
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

