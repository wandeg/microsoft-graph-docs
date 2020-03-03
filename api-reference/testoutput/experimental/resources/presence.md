---
title: "presence resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# presence resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List presences](../api/presence-list.md)|[presence](../resources/presence.md) collection|List properties and relationships of the [presence](../resources/presence.md) objects.|
|[Get presence](../api/presence-get.md)|[presence](../resources/presence.md)|Read properties and relationships of the [presence](../resources/presence.md) object.|
|[Create presence](../api/presence-create.md)|[presence](../resources/presence.md)|Create a new [presence](../resources/presence.md) object.|
|[Delete presence](../api/presence-delete.md)|None|Deletes a [presence](../resources/presence.md).|
|[Update presence](../api/presence-update.md)|[presence](../resources/presence.md)|Update the properties of a [presence](../resources/presence.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|String||
|availability|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.presence",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.presence",
  "id": "String (identifier)",
  "availability": "String",
  "activity": "String"
}
```

