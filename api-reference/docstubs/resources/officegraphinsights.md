---
title: "officeGraphInsights resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# officeGraphInsights resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get officeGraphInsights](../api/officegraphinsights-get.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Read properties and relationships of an [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[Update officeGraphInsights](../api/officegraphinsights-update.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Update the properties of a [officeGraphInsights](../resources/officegraphinsights.md) object.|
|[List trending](../api/officegraphinsights-list-trending.md)|[trending](../resources/trending.md) collection|Get the trendings from the trending navigation property.|
|[Create trending](../api/officegraphinsights-post-trending.md)|[trending](../resources/trending.md)|Create a new trending object.|
|[Delete trending](../api/officegraphinsights-delete-trending.md)|None|Delete a trending object.|
|[Update trending](../api/officegraphinsights-update-trending.md)|[trending](../resources/trending.md)|Update the properties of a trending object.|
|[Get trending](../api/trending-get.md)|[trending](../resources/trending.md)|Read properties and relationships of a [trending](../resources/trending.md) object.|
|[List shared](../api/officegraphinsights-list-shared.md)|[sharedInsight](../resources/sharedinsight.md) collection|Get the sharedInsights from the shared navigation property.|
|[Create shared](../api/officegraphinsights-post-shared.md)|[sharedInsight](../resources/sharedinsight.md)|Create a new shared object.|
|[Delete shared](../api/officegraphinsights-delete-shared.md)|None|Delete a shared object.|
|[Update shared](../api/officegraphinsights-update-shared.md)|[sharedInsight](../resources/sharedinsight.md)|Update the properties of a shared object.|
|[Get sharedInsight](../api/sharedinsight-get.md)|[sharedInsight](../resources/sharedinsight.md)|Read properties and relationships of a [sharedInsight](../resources/sharedinsight.md) object.|
|[List used](../api/officegraphinsights-list-used.md)|[usedInsight](../resources/usedinsight.md) collection|Get the usedInsights from the used navigation property.|
|[Create used](../api/officegraphinsights-post-used.md)|[usedInsight](../resources/usedinsight.md)|Create a new used object.|
|[Delete used](../api/officegraphinsights-delete-used.md)|None|Delete an used object.|
|[Update used](../api/officegraphinsights-update-used.md)|[usedInsight](../resources/usedinsight.md)|Update the properties of an used object.|
|[Get usedInsight](../api/usedinsight-get.md)|[usedInsight](../resources/usedinsight.md)|Read properties and relationships of an [usedInsight](../resources/usedinsight.md) object.|
|[List insights](../api/user-list-insights.md)|[officeGraphInsights](../resources/officegraphinsights.md) collection|Get the officeGraphInsights from the insights navigation property.|
|[Create insights](../api/user-post-insights.md)|[officeGraphInsights](../resources/officegraphinsights.md)|Create a new insights object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|shared|[sharedInsight](../resources/sharedinsight.md) collection|**TODO: Add Description**|
|trending|[trending](../resources/trending.md) collection|**TODO: Add Description**|
|used|[usedInsight](../resources/usedinsight.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeGraphInsights",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeGraphInsights",
  "id": "String (identifier)"
}
```

