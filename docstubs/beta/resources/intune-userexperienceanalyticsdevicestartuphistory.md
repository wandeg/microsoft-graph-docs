---
title: "userExperienceAnalyticsDeviceStartupHistory resource type"
description: "The user experience analytics device startup history entity contains device boot performance history details."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsDeviceStartupHistory resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics device startup history entity contains device boot performance history details.

## Methods

| Method                                                                                                                    | Return Type                                                                                                     | Description                                                                                |
| :------------------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsDeviceStartupHistory](../api/intune-userexperienceanalyticsdevicestartuphistory-list.md)     | [userExperienceAnalyticsDeviceStartupHistory](intune-userExperienceAnalyticsDeviceStartupHistory.md) collection | List properties and relationships of a userExperienceAnalyticsDeviceStartupHistory object. |
| [Create userExperienceAnalyticsDeviceStartupHistory](../api/intune-userexperienceanalyticsdevicestartuphistory-create.md) | [userExperienceAnalyticsDeviceStartupHistory](intune-userExperienceAnalyticsDeviceStartupHistory.md)            | Create a new userExperienceAnalyticsDeviceStartupHistory object.                           |
| [Get userExperienceAnalyticsDeviceStartupHistory](../api/intune-userexperienceanalyticsdevicestartuphistory-get.md)       | [userExperienceAnalyticsDeviceStartupHistory](intune-userExperienceAnalyticsDeviceStartupHistory.md)            | Read properties and relationships of a userExperienceAnalyticsDeviceStartupHistory object. |
| [Update userExperienceAnalyticsDeviceStartupHistory](../api/intune-userexperienceanalyticsdevicestartuphistory-update.md) | [userExperienceAnalyticsDeviceStartupHistory](intune-userExperienceAnalyticsDeviceStartupHistory.md)            | Update the properties of a userExperienceAnalyticsDeviceStartupHistory object.             |
| [Delete userExperienceAnalyticsDeviceStartupHistory](../api/intune-userexperienceanalyticsdevicestartuphistory-delete.md) |                                                                                                                 | Delete a userExperienceAnalyticsDeviceStartupHistory object.                               |

## Properties

| Property                  | Type           | Description                                                                               |
| :------------------------ | :------------- | :---------------------------------------------------------------------------------------- |
| coreBootTimeInMs          | Int32          | The user experience analytics device core boot time in milliseconds.                      |
| coreLoginTimeInMs         | Int32          | The user experience analytics device core login time in milliseconds.                     |
| deviceId                  | String         | The user experience analytics device id.                                                  |
| featureUpdateBootTimeInMs | Int32          | The user experience analytics device feature update time in milliseconds.                 |
| groupPolicyBootTimeInMs   | Int32          | The User experience analytics Device group policy boot time in milliseconds.              |
| groupPolicyLoginTimeInMs  | Int32          | The User experience analytics Device group policy login time in milliseconds.             |
| id                        | String         | The unique identifier of the user experience analytics device startup history. Read-only. |
| isFeatureUpdate           | Boolean        | The user experience analytics device boot record is a feature update.                     |
| isFirstLogin              | Boolean        | The user experience analytics device first login.                                         |
| operatingSystemVersion    | String         | The user experience analytics device boot record's operating system version.              |
| responsiveDesktopTimeInMs | Int32          | The user experience analytics responsive desktop time in milliseconds.                    |
| startTime                 | DateTimeOffset | The user experience analytics device boot start time.                                     |
| totalBootTimeInMs         | Int32          | The user experience analytics device total boot time in milliseconds.                     |
| totalLoginTimeInMs        | Int32          | The user experience analytics device total login time in milliseconds.                    |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "coreBootTimeInMs": "Int32",
  "coreLoginTimeInMs": "Int32",
  "deviceId": "String",
  "featureUpdateBootTimeInMs": "Int32",
  "groupPolicyBootTimeInMs": "Int32",
  "groupPolicyLoginTimeInMs": "Int32",
  "id": "String (identifier)",
  "isFeatureUpdate": "Boolean",
  "isFirstLogin": "Boolean",
  "operatingSystemVersion": "String",
  "responsiveDesktopTimeInMs": "Int32",
  "startTime": "DateTimeOffset",
  "totalBootTimeInMs": "Int32",
  "totalLoginTimeInMs": "Int32"
}
```