---
title: "userExperienceAnalyticsCategory resource type"
description: "The user experience analytics category entity contains the scores and insights for the various metrics of a category."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsCategory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics category entity contains the scores and insights for the various metrics of a category.

## Methods

| Method                                                                                            | Return Type                                                                             | Description                                                                      |
| :------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsCategory](../api/intune-userexperienceanalyticscategory-list.md)     | [userExperienceAnalyticsCategory](intune-userExperienceAnalyticsCategory.md) collection | List properties and relationships of a userExperienceAnalyticsCategory object.   |
| [Create userExperienceAnalyticsCategory](../api/intune-userexperienceanalyticscategory-create.md) | [userExperienceAnalyticsCategory](intune-userExperienceAnalyticsCategory.md)            | Create a new userExperienceAnalyticsCategory object.                             |
| [Get userExperienceAnalyticsCategory](../api/intune-userexperienceanalyticscategory-get.md)       | [userExperienceAnalyticsCategory](intune-userExperienceAnalyticsCategory.md)            | Read properties and relationships of a userExperienceAnalyticsCategory object.   |
| [Update userExperienceAnalyticsCategory](../api/intune-userexperienceanalyticscategory-update.md) | [userExperienceAnalyticsCategory](intune-userExperienceAnalyticsCategory.md)            | Update the properties of a userExperienceAnalyticsCategory object.               |
| [Delete userExperienceAnalyticsCategory](../api/intune-userexperienceanalyticscategory-delete.md) |                                                                                         | Delete a userExperienceAnalyticsCategory object.                                 |
| [List metricValues](../api/intune-userexperienceanalyticscategory-list-metricvalues.md)           | userExperienceAnalyticsMetric                                                           | Get the userExperienceAnalyticsMetric from a metricValues navigation property.   |
| [Create metricValues](../api/intune-userexperienceanalyticscategory-post-metricvalues.md)         | userExperienceAnalyticsMetric                                                           | Create a new metricValues object.                                                |
| [Get metricValues](../api/intune-userexperienceanalyticscategory-get-metricvalues.md)             | userExperienceAnalyticsMetric                                                           | Read the properties and relationships of a userExperienceAnalyticsMetric object. |
| [Update metricValues](../api/intune-userexperienceanalyticscategory-update-metricvalues.md)       | userExperienceAnalyticsMetric                                                           | Update the properties of a metricValues object.                                  |
| [Delete metricValues](../api/intune-userexperienceanalyticscategory-delete-metricvalues.md)       |                                                                                         | Delete a userExperienceAnalyticsMetric object.                                   |

## Properties

| Property     | Type                                                                                        | Description                                                                 |
| :----------- | :------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------- |
| id           | String                                                                                      | The unique identifier of the user experience analytics category. Read-only. |
| insights     | [userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection | The insights for the user experience analytics category.                    |
| overallScore | Int32                                                                                       | The overall score of the user experience analytics category.                |
| state        | String                                                                                      | The current health state of the user experience analytics category.         |

## Relationships

| Relationship | Type                                                                                      | Description                                                   |
| :----------- | :---------------------------------------------------------------------------------------- | :------------------------------------------------------------ |
| metricValues | [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection | The metric values for the user experience analytics category. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "insights": [{"@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"}],
  "overallScore": "Int32",
  "state": "unknown | insufficientData | needsAttention | meetingGoals"
}
```