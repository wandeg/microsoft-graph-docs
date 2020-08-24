---
title: "userExperienceAnalyticsScoreHistory resource type"
description: "The user experience analytics device startup score history."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsScoreHistory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics device startup score history.

## Methods

| Method                                                                                                    | Return Type                                                                                     | Description                                                                        |
| :-------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsScoreHistory](../api/intune-userexperienceanalyticsscorehistory-list.md)     | [userExperienceAnalyticsScoreHistory](intune-userExperienceAnalyticsScoreHistory.md) collection | List properties and relationships of a userExperienceAnalyticsScoreHistory object. |
| [Create userExperienceAnalyticsScoreHistory](../api/intune-userexperienceanalyticsscorehistory-create.md) | [userExperienceAnalyticsScoreHistory](intune-userExperienceAnalyticsScoreHistory.md)            | Create a new userExperienceAnalyticsScoreHistory object.                           |
| [Get userExperienceAnalyticsScoreHistory](../api/intune-userexperienceanalyticsscorehistory-get.md)       | [userExperienceAnalyticsScoreHistory](intune-userExperienceAnalyticsScoreHistory.md)            | Read properties and relationships of a userExperienceAnalyticsScoreHistory object. |
| [Update userExperienceAnalyticsScoreHistory](../api/intune-userexperienceanalyticsscorehistory-update.md) | [userExperienceAnalyticsScoreHistory](intune-userExperienceAnalyticsScoreHistory.md)            | Update the properties of a userExperienceAnalyticsScoreHistory object.             |
| [Delete userExperienceAnalyticsScoreHistory](../api/intune-userexperienceanalyticsscorehistory-delete.md) |                                                                                                 | Delete a userExperienceAnalyticsScoreHistory object.                               |

## Properties

| Property                 | Type           | Description                                                                               |
| :----------------------- | :------------- | :---------------------------------------------------------------------------------------- |
| coreBootScore            | Int32          | The user experience analytics device core boot score.                                     |
| coreSigninScore          | Int32          | The User experience analytics device core sign-in score.                                  |
| id                       | String         | The unique identifier of the user experience analytics device startup process. Read-only. |
| recommendedSoftwareScore | Int32          | The User experience analytics device core sign-in score.                                  |
| startupDateTime          | DateTimeOffset | The user experience analytics device startup date time.                                   |
| startupScore             | Int32          | User experience analytics device startup score.                                           |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsScoreHistory",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "coreBootScore": "Int32",
  "coreSigninScore": "Int32",
  "id": "String (identifier)",
  "recommendedSoftwareScore": "Int32",
  "startupDateTime": "DateTimeOffset",
  "startupScore": "Int32"
}
```