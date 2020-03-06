---
title: "userExperienceAnalyticsMetric resource type"
description: "The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsMetric resource type


Namespace: microsoft.graph

The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[List metricValues](../api/userexperienceanalyticscategory-list-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the metricValues navigation property.|
|[Add metricValues](../api/userexperienceanalyticscategory-post-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Add metricValues by posting to the metricValues collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|unit|String|The unit of the user experience analytics metric.|
|value|Double|The value of the user experience analytics metric.|

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

