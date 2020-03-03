---
title: "trending resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# trending resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List trendings](../api/trending-list.md)|[trending](../resources/trending.md) collection|List properties and relationships of the [trending](../resources/trending.md) objects.|
|[Get trending](../api/trending-get.md)|[trending](../resources/trending.md)|Read properties and relationships of the [trending](../resources/trending.md) object.|
|[Create trending](../api/trending-create.md)|[trending](../resources/trending.md)|Create a new [trending](../resources/trending.md) object.|
|[Delete trending](../api/trending-delete.md)|None|Deletes a [trending](../resources/trending.md).|
|[Update trending](../api/trending-update.md)|[trending](../resources/trending.md)|Update the properties of a [trending](../resources/trending.md) object.|
|[Get entity](../api/entity-get.md)|[entity](../resources/entity.md)|Read properties and relationships of the [entity](../resources/entity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|resourceReference|[resourceReference](../resources/resourcereference.md)||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||
|weight|Double||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[entity](../resources/entity.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.trending",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trending",
  "id": "String (identifier)",
  "weight": "Double",
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization",
    "title": "String",
    "type": "String",
    "mediaType": "String",
    "previewImageUrl": "String",
    "previewText": "String",
    "containerWebUrl": "String",
    "containerDisplayName": "String",
    "containerType": "String"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference",
    "webUrl": "String",
    "id": "String"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

