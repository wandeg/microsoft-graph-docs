---
title: "userExperienceAnalyticsOverview resource type"
description: "The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsOverview resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.

## Methods

| Method                                                                                            | Return Type                                                                             | Description                                                                    |
| :------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| [List userExperienceAnalyticsOverview](../api/intune-userexperienceanalyticsoverview-list.md)     | [userExperienceAnalyticsOverview](intune-userExperienceAnalyticsOverview.md) collection | List properties and relationships of a userExperienceAnalyticsOverview object. |
| [Create userExperienceAnalyticsOverview](../api/intune-userexperienceanalyticsoverview-create.md) | [userExperienceAnalyticsOverview](intune-userExperienceAnalyticsOverview.md)            | Create a new userExperienceAnalyticsOverview object.                           |
| [Get userExperienceAnalyticsOverview](../api/intune-userexperienceanalyticsoverview-get.md)       | [userExperienceAnalyticsOverview](intune-userExperienceAnalyticsOverview.md)            | Read properties and relationships of a userExperienceAnalyticsOverview object. |
| [Update userExperienceAnalyticsOverview](../api/intune-userexperienceanalyticsoverview-update.md) | [userExperienceAnalyticsOverview](intune-userExperienceAnalyticsOverview.md)            | Update the properties of a userExperienceAnalyticsOverview object.             |
| [Delete userExperienceAnalyticsOverview](../api/intune-userexperienceanalyticsoverview-delete.md) |                                                                                         | Delete a userExperienceAnalyticsOverview object.                               |

## Properties

| Property                          | Type                                                                                        | Description                                                                           |
| :-------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------ |
| bestPracticesHealthState          | String                                                                                      | The current health state of the user experience analytics 'BestPractices' category.   |
| bestPracticesOverallScore         | Int32                                                                                       | The user experience analytics best practices overall score.                           |
| deviceBootPerformanceHealthState  | String                                                                                      | The current health state of the user experience analytics 'BootPerformance' category. |
| deviceBootPerformanceOverallScore | Int32                                                                                       | The user experience analytics device boot performance overall score.                  |
| id                                | String                                                                                      | The unique identifier of the user experience analytics overview. Read-only.           |
| insights                          | [userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection | The user experience analytics insights.                                               |
| overallScore                      | Int32                                                                                       | The user experience analytics overall score.                                          |
| state                             | String                                                                                      | The current health state of the user experience analytics overview.                   |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "bestPracticesHealthState": "unknown | insufficientData | needsAttention | meetingGoals",
  "bestPracticesOverallScore": "Int32",
  "deviceBootPerformanceHealthState": "unknown | insufficientData | needsAttention | meetingGoals",
  "deviceBootPerformanceOverallScore": "Int32",
  "id": "String (identifier)",
  "insights": [{"@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"}],
  "overallScore": "Int32",
  "state": "unknown | insufficientData | needsAttention | meetingGoals"
}
```