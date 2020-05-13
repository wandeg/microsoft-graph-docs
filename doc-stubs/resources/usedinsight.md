---
title: "usedInsight resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# usedInsight resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List used](../api/officegraphinsights-list-used.md)|[usedInsight](../resources/usedinsight.md) collection|Get the usedInsights from the used navigation property.|
|[Create used](../api/officegraphinsights-post-used.md)|[usedInsight](../resources/usedinsight.md)|Create a new used object.|
|[Delete used](../api/officegraphinsights-delete-used.md)|None|Delete an [usedInsight](../resources/usedinsight.md) object.|
|[Update used](../api/officegraphinsights-update-used.md)|[usedInsight](../resources/usedinsight.md)|Update the properties of an used object.|
|[Get used](../api/officegraphinsights-get-usedinsight.md)|[usedInsight](../resources/usedinsight.md)|Read the properties and relationships of an [usedInsight](../resources/usedinsight.md) object.|
|[List resource](../api/usedinsight-list-resource.md)|[entity](../resources/entity.md) collection|Get the entities from the resource navigation property.|
|[Add resource](../api/usedinsight-post-resource.md)|[entity](../resources/entity.md)|Add resource by posting to the resource collection.|
|[Remove resource](../api/usedinsight-delete-resource.md)|None|Remove an [entity](../resources/entity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastUsed|[usageDetails](../resources/usagedetails.md)|**TODO: Add Description**|
|resourceReference|[resourceReference](../resources/resourcereference.md)|**TODO: Add Description**|
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[entity](../resources/entity.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usedInsight",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usedInsight",
  "id": "String (identifier)",
  "lastUsed": {
    "@odata.type": "microsoft.graph.usageDetails"
  },
  "resourceVisualization": {
    "@odata.type": "microsoft.graph.resourceVisualization"
  },
  "resourceReference": {
    "@odata.type": "microsoft.graph.resourceReference"
  }
}
```

