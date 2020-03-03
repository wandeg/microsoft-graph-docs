---
title: "userExperienceAnalyticsRegressionSummary resource type"
description: "The user experience analytics Regression Summary."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userExperienceAnalyticsRegressionSummary resource type

The user experience analytics Regression Summary.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsRegressionSummaries](../api/intune-devices-userexperienceanalyticsregressionsummary-list.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md) collection|List properties and relationships of the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) objects.|
|[Get userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-get.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Read properties and relationships of the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[Create userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-create.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Create a new [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[Delete userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-delete.md)|None|Deletes a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md).|
|[Update userExperienceAnalyticsRegressionSummary](../api/intune-devices-userexperienceanalyticsregressionsummary-update.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.|
|[summarizeDeviceRegressionPerformance](../api/intune-devices-userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)||
|[List modelRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-list-modelregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|Get the userExperienceAnalyticsMetrics from the modelRegression navigation property.|
|[Add modelRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-post-modelregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md)|Add modelRegression by posting to the modelRegression collection.|
|[List manufacturerRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-list-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|Get the userExperienceAnalyticsMetrics from the manufacturerRegression navigation property.|
|[Add manufacturerRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-post-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md)|Add manufacturerRegression by posting to the manufacturerRegression collection.|
|[List operatingSystemRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-list-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|Get the userExperienceAnalyticsMetrics from the operatingSystemRegression navigation property.|
|[Add operatingSystemRegression](../api/intune-devices-userexperienceanalyticsregressionsummary-post-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md)|Add operatingSystemRegression by posting to the operatingSystemRegression collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|manufacturerRegression|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|The metric values for the user experience analytics Manufacturer regression.|
|modelRegression|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|The metric values for the user experience analytics model regression.|
|operatingSystemRegression|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|The metric values for the user experience analytics operating system regression.|

## JSON Representation
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

