---
title: "presence resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# presence resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get presence](../api/presence-get.md)|[presence](../resources/presence.md)|Read properties and relationships of the [presence](../resources/presence.md) object.|
|[Update presence](../api/presence-update.md)|[presence](../resources/presence.md)|Update the properties of a [presence](../resources/presence.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|String||
|availability|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
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

