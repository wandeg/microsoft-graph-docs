---
title: "audioRoutingGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# audioRoutingGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get audioRoutingGroup](../api/audioroutinggroup-get.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Read the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.|
|[Update audioRoutingGroup](../api/audioroutinggroup-update.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Update the properties of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|receivers|String collection|**TODO: Add Description**|
|routingMode|routingMode|**TODO: Add Description**. Possible values are: `oneToOne`, `multicast`.|
|sources|String collection|**TODO: Add Description**|

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

