---
title: "audioRoutingGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# audioRoutingGroup resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get audioRoutingGroup](../api/audioroutinggroup-get.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Read properties and relationships of the [audioRoutingGroup](../resources/audioroutinggroup.md) object.|
|[Update audioRoutingGroup](../api/audioroutinggroup-update.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Update the properties of a [audioRoutingGroup](../resources/audioroutinggroup.md) object.|
|[List audioRoutingGroups](../api/call-list-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md) collection|Get the audioRoutingGroups from the audioRoutingGroups navigation property.|
|[Add audioRoutingGroups](../api/call-post-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Add audioRoutingGroups by posting to the audioRoutingGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|receivers|String collection||
|routingMode|Enumeration|. Possible values are: `oneToOne`, `multicast`.|
|sources|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.audioRoutingGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "id": "String (identifier)",
  "routingMode": "String",
  "sources": [
    "String"
  ],
  "receivers": [
    "String"
  ]
}
```

