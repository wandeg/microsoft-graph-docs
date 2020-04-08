---
title: "userExperienceAnalyticsMetric resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsMetric resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|unit|String||
|value|Double||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "Double",
  "unit": "String"
}
```

