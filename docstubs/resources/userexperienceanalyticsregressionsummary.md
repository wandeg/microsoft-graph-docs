---
title: "userExperienceAnalyticsRegressionSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsRegressionSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsRegressionSummary](../api/userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Read properties and relationships of the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[Update userExperienceAnalyticsRegressionSummary](../api/userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[summarizeDeviceRegressionPerformance](../api/userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)||
|[List modelRegression](../api/userexperienceanalyticsregressionsummary-list-modelregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the modelRegression navigation property.|
|[Add modelRegression](../api/userexperienceanalyticsregressionsummary-post-modelregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Add modelRegression by posting to the modelRegression collection.|
|[List manufacturerRegression](../api/userexperienceanalyticsregressionsummary-list-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the manufacturerRegression navigation property.|
|[Add manufacturerRegression](../api/userexperienceanalyticsregressionsummary-post-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Add manufacturerRegression by posting to the manufacturerRegression collection.|
|[List operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-list-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the operatingSystemRegression navigation property.|
|[Add operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-post-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Add operatingSystemRegression by posting to the operatingSystemRegression collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|manufacturerRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection||
|modelRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection||
|operatingSystemRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```

