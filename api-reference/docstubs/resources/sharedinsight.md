---
title: "sharedInsight resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# sharedInsight resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sharedInsight](../api/sharedinsight-get.md)|[sharedInsight](../resources/sharedinsight.md)|Read properties and relationships of a [sharedInsight](../resources/sharedinsight.md) object.|
|[Update sharedInsight](../api/sharedinsight-update.md)|[sharedInsight](../resources/sharedinsight.md)|Update the properties of a [sharedInsight](../resources/sharedinsight.md) object.|
|[List lastSharedMethod](../api/sharedinsight-list-lastsharedmethod.md)|[entity](../resources/entity.md) collection|Get the entities from the lastSharedMethod navigation property.|
|[Add lastSharedMethod](../api/sharedinsight-post-lastsharedmethod.md)|[entity](../resources/entity.md)|Add lastSharedMethod by posting to the lastSharedMethod collection.|
|[Remove lastSharedMethod](../api/sharedinsight-delete-lastsharedmethod.md)|None|Remove a lastSharedMethod object.|
|[List resource](../api/sharedinsight-list-resource.md)|[entity](../resources/entity.md) collection|Get the entities from the resource navigation property.|
|[Add resource](../api/sharedinsight-post-resource.md)|[entity](../resources/entity.md)|Add resource by posting to the resource collection.|
|[Remove resource](../api/sharedinsight-delete-resource.md)|None|Remove a resource object.|
|[List shared](../api/officegraphinsights-list-shared.md)|[sharedInsight](../resources/sharedinsight.md) collection|Get the sharedInsights from the shared navigation property.|
|[Create shared](../api/officegraphinsights-post-shared.md)|[sharedInsight](../resources/sharedinsight.md)|Create a new shared object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingdetail.md)|**TODO: Add Description**|
|resourceReference|[resourceReference](../resources/resourcereference.md)|**TODO: Add Description**|
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)|**TODO: Add Description**|
|sharingHistory|[sharingDetail](../resources/sharingdetail.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|lastSharedMethod|[entity](../resources/entity.md)|**TODO: Add Description**|
|resource|[entity](../resources/entity.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "String (identifier)",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "String",
      "id": "String",
      "address": "String"
    },
    "sharedDateTime": "String (timestamp)",
    "sharingSubject": "String",
    "sharingType": "String",
    "sharingReference": {
      "@odata.type": "microsoft.graph.resourceReference",
      "webUrl": "String",
      "type": "String"
    }
  },
  "sharingHistory": [
    {
      "@odata.type": "microsoft.graph.sharingDetail"
    }
  ],
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization",
    "title": "String",
    "mediaType": "String",
    "previewImageUrl": "String",
    "previewText": "String",
    "containerWebUrl": "String",
    "containerDisplayName": "String",
    "containerType": "String"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  }
}
```

