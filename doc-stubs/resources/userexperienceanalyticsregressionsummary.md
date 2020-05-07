---
title: "userExperienceAnalyticsRegressionSummary resource type"
description: "The user experience analytics Regression Summary."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsRegressionSummary resource type


Namespace: microsoft.graph

The user experience analytics Regression Summary.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[summarizeDeviceRegressionPerformance](../api/userexperienceanalyticsregressionsummary-summarizedeviceregressionperformance.md)|[userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md)|**TODO: Add Description**|
|[List modelRegression](../api/userexperienceanalyticsregressionsummary-list-modelregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the modelRegression navigation property.|
|[Create modelRegression](../api/userexperienceanalyticsregressionsummary-post-modelregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Create a new modelRegression object.|
|[Delete modelRegression](../api/userexperienceanalyticsregressionsummary-delete-modelregression.md)|None|Delete a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update modelRegression](../api/userexperienceanalyticsregressionsummary-update-modelregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a modelRegression object.|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read the properties and relationships of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[List manufacturerRegression](../api/userexperienceanalyticsregressionsummary-list-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the manufacturerRegression navigation property.|
|[Create manufacturerRegression](../api/userexperienceanalyticsregressionsummary-post-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Create a new manufacturerRegression object.|
|[Delete manufacturerRegression](../api/userexperienceanalyticsregressionsummary-delete-manufacturerregression.md)|None|Delete a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update manufacturerRegression](../api/userexperienceanalyticsregressionsummary-update-manufacturerregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a manufacturerRegression object.|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read the properties and relationships of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[List operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-list-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the operatingSystemRegression navigation property.|
|[Create operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-post-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Create a new operatingSystemRegression object.|
|[Delete operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-delete-operatingsystemregression.md)|None|Delete an [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update operatingSystemRegression](../api/userexperienceanalyticsregressionsummary-update-operatingsystemregression.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of an operatingSystemRegression object.|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read the properties and relationships of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics regression summary.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|manufacturerRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|The metric values for the user experience analytics Manufacturer regression.|
|modelRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|The metric values for the user experience analytics model regression.|
|operatingSystemRegression|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|The metric values for the user experience analytics operating system regression.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsRegressionSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```

