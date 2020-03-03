---
title: "usedInsight resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# usedInsight resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List usedInsights](../api/usedinsight-list.md)|[usedInsight](../resources/usedinsight.md) collection|List properties and relationships of the [usedInsight](../resources/usedinsight.md) objects.|
|[Get usedInsight](../api/usedinsight-get.md)|[usedInsight](../resources/usedinsight.md)|Read properties and relationships of the [usedInsight](../resources/usedinsight.md) object.|
|[Create usedInsight](../api/usedinsight-create.md)|[usedInsight](../resources/usedinsight.md)|Create a new [usedInsight](../resources/usedinsight.md) object.|
|[Delete usedInsight](../api/usedinsight-delete.md)|None|Deletes a [usedInsight](../resources/usedinsight.md).|
|[Update usedInsight](../api/usedinsight-update.md)|[usedInsight](../resources/usedinsight.md)|Update the properties of a [usedInsight](../resources/usedinsight.md) object.|
|[Get entity](../api/entity-get.md)|[entity](../resources/entity.md)|Read properties and relationships of the [entity](../resources/entity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUsed|[usageDetails](../resources/usagedetails.md)||
|resourceReference|[resourceReference](../resources/resourcereference.md)||
|resourceVisualization|[resourceVisualization](../resources/resourcevisualization.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[entity](../resources/entity.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.usageDetails",
    "lastAccessedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  },
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
  }
}
```

