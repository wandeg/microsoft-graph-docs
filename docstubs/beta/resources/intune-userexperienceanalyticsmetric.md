---
title: "userExperienceAnalyticsMetric resource type"
description: "The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsMetric resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.

## Methods

| Method                                                                                        | Return Type                                                                         | Description                                                                  |
| :-------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- | :--------------------------------------------------------------------------- |
| [List userExperienceAnalyticsMetric](../api/intune-userexperienceanalyticsmetric-list.md)     | [userExperienceAnalyticsMetric](intune-userExperienceAnalyticsMetric.md) collection | List properties and relationships of a userExperienceAnalyticsMetric object. |
| [Create userExperienceAnalyticsMetric](../api/intune-userexperienceanalyticsmetric-create.md) | [userExperienceAnalyticsMetric](intune-userExperienceAnalyticsMetric.md)            | Create a new userExperienceAnalyticsMetric object.                           |
| [Get userExperienceAnalyticsMetric](../api/intune-userexperienceanalyticsmetric-get.md)       | [userExperienceAnalyticsMetric](intune-userExperienceAnalyticsMetric.md)            | Read properties and relationships of a userExperienceAnalyticsMetric object. |
| [Update userExperienceAnalyticsMetric](../api/intune-userexperienceanalyticsmetric-update.md) | [userExperienceAnalyticsMetric](intune-userExperienceAnalyticsMetric.md)            | Update the properties of a userExperienceAnalyticsMetric object.             |
| [Delete userExperienceAnalyticsMetric](../api/intune-userexperienceanalyticsmetric-delete.md) |                                                                                     | Delete a userExperienceAnalyticsMetric object.                               |

## Properties

| Property | Type   | Description                                                               |
| :------- | :----- | :------------------------------------------------------------------------ |
| id       | String | The unique identifier of the user experience analytics metric. Read-only. |
| unit     | String | The unit of the user experience analytics metric.                         |
| value    | Double | The value of the user experience analytics metric.                        |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "unit": "String",
  "value": "Double"
}
```