---
title: "plannerBucketTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerBucketTaskBoardTaskFormat resource type


Namespace: microsoft.graph




Inherits from [plannerDelta](../resources/plannerdelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerBucketTaskBoardTaskFormats](../api/plannerbuckettaskboardtaskformat-list.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) collection|List properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) objects.|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Read properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|
|[Create plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-create.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Create a new [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|
|[Delete plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-delete.md)|None|Deletes a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md).|
|[Update plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-update.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Update the properties of a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|

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

