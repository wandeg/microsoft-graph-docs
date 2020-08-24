---
title: "userExperienceAnalyticsRegressionSummary resource type"
description: "The user experience analytics Regression Summary."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsRegressionSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics Regression Summary.

## Methods

| Method                                                                                                                                 | Return Type                                                                                               | Description                                                                                  |
| :------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsRegressionSummary](../api/intune-userexperienceanalyticsregressionsummary-list.md)                        | [userExperienceAnalyticsRegressionSummary](intune-userExperienceAnalyticsRegressionSummary.md) collection | List properties and relationships of a userExperienceAnalyticsRegressionSummary object.      |
| [Create userExperienceAnalyticsRegressionSummary](../api/intune-userexperienceanalyticsregressionsummary-create.md)                    | [userExperienceAnalyticsRegressionSummary](intune-userExperienceAnalyticsRegressionSummary.md)            | Create a new userExperienceAnalyticsRegressionSummary object.                                |
| [Get userExperienceAnalyticsRegressionSummary](../api/intune-userexperienceanalyticsregressionsummary-get.md)                          | [userExperienceAnalyticsRegressionSummary](intune-userExperienceAnalyticsRegressionSummary.md)            | Read properties and relationships of a userExperienceAnalyticsRegressionSummary object.      |
| [Update userExperienceAnalyticsRegressionSummary](../api/intune-userexperienceanalyticsregressionsummary-update.md)                    | [userExperienceAnalyticsRegressionSummary](intune-userExperienceAnalyticsRegressionSummary.md)            | Update the properties of a userExperienceAnalyticsRegressionSummary object.                  |
| [Delete userExperienceAnalyticsRegressionSummary](../api/intune-userexperienceanalyticsregressionsummary-delete.md)                    |                                                                                                           | Delete a userExperienceAnalyticsRegressionSummary object.                                    |
| [summarizeDeviceRegressionPerformance](../api/intune-userexperienceanalyticsregressionsummary-summarizeDeviceRegressionPerformance.md) | userExperienceAnalyticsRegressionSummary                                                                  |                                                                                              |
| [List manufacturerRegression](../api/intune-userexperienceanalyticsregressionsummary-list-manufacturerregression.md)                   | userExperienceAnalyticsMetric                                                                             | Get the userExperienceAnalyticsMetric from a manufacturerRegression navigation property.     |
| [Create manufacturerRegression](../api/intune-userexperienceanalyticsregressionsummary-post-manufacturerregression.md)                 | userExperienceAnalyticsMetric                                                                             | Create a new manufacturerRegression object.                                                  |
| [Get manufacturerRegression](../api/intune-userexperienceanalyticsregressionsummary-get-manufacturerregression.md)                     | userExperienceAnalyticsMetric                                                                             | Read the properties and relationships of a userExperienceAnalyticsMetric object.             |
| [Update manufacturerRegression](../api/intune-userexperienceanalyticsregressionsummary-update-manufacturerregression.md)               | userExperienceAnalyticsMetric                                                                             | Update the properties of a manufacturerRegression object.                                    |
| [Delete manufacturerRegression](../api/intune-userexperienceanalyticsregressionsummary-delete-manufacturerregression.md)               |                                                                                                           | Delete a userExperienceAnalyticsMetric object.                                               |
| [List modelRegression](../api/intune-userexperienceanalyticsregressionsummary-list-modelregression.md)                                 | userExperienceAnalyticsMetric                                                                             | Get the userExperienceAnalyticsMetric from a modelRegression navigation property.            |
| [Create modelRegression](../api/intune-userexperienceanalyticsregressionsummary-post-modelregression.md)                               | userExperienceAnalyticsMetric                                                                             | Create a new modelRegression object.                                                         |
| [Get modelRegression](../api/intune-userexperienceanalyticsregressionsummary-get-modelregression.md)                                   | userExperienceAnalyticsMetric                                                                             | Read the properties and relationships of a userExperienceAnalyticsMetric object.             |
| [Update modelRegression](../api/intune-userexperienceanalyticsregressionsummary-update-modelregression.md)                             | userExperienceAnalyticsMetric                                                                             | Update the properties of a modelRegression object.                                           |
| [Delete modelRegression](../api/intune-userexperienceanalyticsregressionsummary-delete-modelregression.md)                             |                                                                                                           | Delete a userExperienceAnalyticsMetric object.                                               |
| [List operatingSystemRegression](../api/intune-userexperienceanalyticsregressionsummary-list-operatingsystemregression.md)             | userExperienceAnalyticsMetric                                                                             | Get the userExperienceAnalyticsMetric from an operatingSystemRegression navigation property. |
| [Create operatingSystemRegression](../api/intune-userexperienceanalyticsregressionsummary-post-operatingsystemregression.md)           | userExperienceAnalyticsMetric                                                                             | Create a new operatingSystemRegression object.                                               |
| [Get operatingSystemRegression](../api/intune-userexperienceanalyticsregressionsummary-get-operatingsystemregression.md)               | userExperienceAnalyticsMetric                                                                             | Read the properties and relationships of a userExperienceAnalyticsMetric object.             |
| [Update operatingSystemRegression](../api/intune-userexperienceanalyticsregressionsummary-update-operatingsystemregression.md)         | userExperienceAnalyticsMetric                                                                             | Update the properties of an operatingSystemRegression object.                                |
| [Delete operatingSystemRegression](../api/intune-userexperienceanalyticsregressionsummary-delete-operatingsystemregression.md)         |                                                                                                           | Delete a userExperienceAnalyticsMetric object.                                               |

## Properties

| Property | Type   | Description                                                                           |
| :------- | :----- | :------------------------------------------------------------------------------------ |
| id       | String | The unique identifier of the user experience analytics regression summary. Read-only. |

## Relationships

| Relationship              | Type                                                                                      | Description                                                                      |
| :------------------------ | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| manufacturerRegression    | [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection | The metric values for the user experience analytics Manufacturer regression.     |
| modelRegression           | [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection | The metric values for the user experience analytics model regression.            |
| operatingSystemRegression | [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection | The metric values for the user experience analytics operating system regression. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "String (identifier)"
}
```