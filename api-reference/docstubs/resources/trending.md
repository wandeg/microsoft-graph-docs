---
title: "trending resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# trending resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get trending](../api/trending-get.md)|[trending](../resources/trending.md)|Read the properties and relationships of a [trending](../resources/trending.md) object.|
|[Update trending](../api/trending-update.md)|[trending](../resources/trending.md)|Update the properties of a [trending](../resources/trending.md) object.|
|[List resource](../api/trending-list-resource.md)|[entity](../resources/entity.md) collection|Get the entities from the resource navigation property.|
|[Add resource](../api/trending-post-resource.md)|[entity](../resources/entity.md)|Add resource by posting to the resource collection.|
|[Remove resource](../api/trending-delete-resource.md)|None|Remove a [entity](../resources/entity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourceReference|[resourceReference](../resources/resourcereference.md)|**TODO: Add Description**|
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)|**TODO: Add Description**|
|weight|Double|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[entity](../resources/entity.md)|**TODO: Add Description**|

## JSON representation
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

