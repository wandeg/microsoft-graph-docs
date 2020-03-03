---
title: "plannerProgressTaskBoardTaskFormat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerProgressTaskBoardTaskFormat resource type




Inherits from [plannerDelta](../resources/plannerDelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerProgressTaskBoardTaskFormats](../api/plannerprogresstaskboardtaskformat-list.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md) collection|List properties and relationships of the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) objects.|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Create plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-create.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md)|Create a new [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Delete plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-delete.md)|None|Deletes a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md).|
|[Update plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-update.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md)|Update the properties of a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|

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
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "id": "String (identifier)",
  "orderHint": "String"
}
```

