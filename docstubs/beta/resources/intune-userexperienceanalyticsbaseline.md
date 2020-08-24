---
title: "userExperienceAnalyticsBaseline resource type"
description: "The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsBaseline resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.

## Methods

| Method                                                                                                                      | Return Type                                                                             | Description                                                                                      |
| :-------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsBaseline](../api/intune-userexperienceanalyticsbaseline-list.md)                               | [userExperienceAnalyticsBaseline](intune-userExperienceAnalyticsBaseline.md) collection | List properties and relationships of a userExperienceAnalyticsBaseline object.                   |
| [Create userExperienceAnalyticsBaseline](../api/intune-userexperienceanalyticsbaseline-create.md)                           | [userExperienceAnalyticsBaseline](intune-userExperienceAnalyticsBaseline.md)            | Create a new userExperienceAnalyticsBaseline object.                                             |
| [Get userExperienceAnalyticsBaseline](../api/intune-userexperienceanalyticsbaseline-get.md)                                 | [userExperienceAnalyticsBaseline](intune-userExperienceAnalyticsBaseline.md)            | Read properties and relationships of a userExperienceAnalyticsBaseline object.                   |
| [Update userExperienceAnalyticsBaseline](../api/intune-userexperienceanalyticsbaseline-update.md)                           | [userExperienceAnalyticsBaseline](intune-userExperienceAnalyticsBaseline.md)            | Update the properties of a userExperienceAnalyticsBaseline object.                               |
| [Delete userExperienceAnalyticsBaseline](../api/intune-userexperienceanalyticsbaseline-delete.md)                           |                                                                                         | Delete a userExperienceAnalyticsBaseline object.                                                 |
| [List bestPracticesMetrics](../api/intune-userexperienceanalyticsbaseline-list-bestpracticesmetrics.md)                     | userExperienceAnalyticsCategory                                                         | Get the userExperienceAnalyticsCategory from a bestPracticesMetrics navigation property.         |
| [Add bestPracticesMetrics](../api/intune-userexperienceanalyticsbaseline-post-bestpracticesmetrics.md)                      | userExperienceAnalyticsCategory                                                         | Add bestPracticesMetrics by posting to the bestPracticesMetrics collection.                      |
| [Get bestPracticesMetrics](../api/intune-userexperienceanalyticsbaseline-get-bestpracticesmetrics.md)                       | userExperienceAnalyticsCategory                                                         | Read the properties and relationships of a userExperienceAnalyticsCategory object.               |
| [Update bestPracticesMetrics](../api/intune-userexperienceanalyticsbaseline-update-bestpracticesmetrics.md)                 | userExperienceAnalyticsCategory                                                         | Update the properties of a bestPracticesMetrics object.                                          |
| [Remove bestPracticesMetrics](../api/intune-userexperienceanalyticsbaseline-delete-bestpracticesmetrics.md)                 |                                                                                         | Remove a userExperienceAnalyticsCategory object.                                                 |
| [List deviceBootPerformanceMetrics](../api/intune-userexperienceanalyticsbaseline-list-devicebootperformancemetrics.md)     | userExperienceAnalyticsCategory                                                         | Get the userExperienceAnalyticsCategory from a deviceBootPerformanceMetrics navigation property. |
| [Add deviceBootPerformanceMetrics](../api/intune-userexperienceanalyticsbaseline-post-devicebootperformancemetrics.md)      | userExperienceAnalyticsCategory                                                         | Add deviceBootPerformanceMetrics by posting to the deviceBootPerformanceMetrics collection.      |
| [Get deviceBootPerformanceMetrics](../api/intune-userexperienceanalyticsbaseline-get-devicebootperformancemetrics.md)       | userExperienceAnalyticsCategory                                                         | Read the properties and relationships of a userExperienceAnalyticsCategory object.               |
| [Update deviceBootPerformanceMetrics](../api/intune-userexperienceanalyticsbaseline-update-devicebootperformancemetrics.md) | userExperienceAnalyticsCategory                                                         | Update the properties of a deviceBootPerformanceMetrics object.                                  |
| [Remove deviceBootPerformanceMetrics](../api/intune-userexperienceanalyticsbaseline-delete-devicebootperformancemetrics.md) |                                                                                         | Remove a userExperienceAnalyticsCategory object.                                                 |

## Properties

| Property        | Type           | Description                                                                               |
| :-------------- | :------------- | :---------------------------------------------------------------------------------------- |
| createdDateTime | DateTimeOffset | The date the custom baseline was created.                                                 |
| displayName     | String         | The name of the user experience analytics baseline.                                       |
| id              | String         | The unique identifier of the user experience analytics baseline. Read-only.               |
| isBuiltIn       | Boolean        | Signifies if the current baseline is the commercial median baseline or a custom baseline. |
| overallScore    | Int32          | The overall score of the user experience analytics baseline.                              |

## Relationships

| Relationship                 | Type                                                                               | Description                                                    |
| :--------------------------- | :--------------------------------------------------------------------------------- | :------------------------------------------------------------- |
| bestPracticesMetrics         | [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) | The user experience analytics best practices metrics.          |
| deviceBootPerformanceMetrics | [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) | The user experience analytics device boot performance metrics. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "createdDateTime": "DateTimeOffset",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": "Boolean",
  "overallScore": "Int32"
}
```