---
title: "plannerBucketTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerBucketTaskBoardTaskFormat resource type




Inherits from [plannerDelta](../resources/plannerDelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerBucketTaskBoardTaskFormats](../api/plannerbuckettaskboardtaskformat-list.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md) collection|List properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) objects.|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|
|[Create plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-create.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md)|Create a new [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|
|[Delete plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-delete.md)|None|Deletes a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md).|
|[Update plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-update.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md)|Update the properties of a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "id": "String (identifier)",
  "orderHint": "String"
}
```

