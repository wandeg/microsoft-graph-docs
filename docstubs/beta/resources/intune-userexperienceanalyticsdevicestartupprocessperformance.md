---
title: "userExperienceAnalyticsDeviceStartupProcessPerformance resource type"
description: "The user experience analytics device startup process performance."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsDeviceStartupProcessPerformance resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics device startup process performance.

## Methods

| Method                                                                                                                                          | Return Type                                                                                                                           | Description                                                                                           |
| :---------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-userexperienceanalyticsdevicestartupprocessperformance-list.md)     | [userExperienceAnalyticsDeviceStartupProcessPerformance](intune-userExperienceAnalyticsDeviceStartupProcessPerformance.md) collection | List properties and relationships of a userExperienceAnalyticsDeviceStartupProcessPerformance object. |
| [Create userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-userexperienceanalyticsdevicestartupprocessperformance-create.md) | [userExperienceAnalyticsDeviceStartupProcessPerformance](intune-userExperienceAnalyticsDeviceStartupProcessPerformance.md)            | Create a new userExperienceAnalyticsDeviceStartupProcessPerformance object.                           |
| [Get userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-userexperienceanalyticsdevicestartupprocessperformance-get.md)       | [userExperienceAnalyticsDeviceStartupProcessPerformance](intune-userExperienceAnalyticsDeviceStartupProcessPerformance.md)            | Read properties and relationships of a userExperienceAnalyticsDeviceStartupProcessPerformance object. |
| [Update userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-userexperienceanalyticsdevicestartupprocessperformance-update.md) | [userExperienceAnalyticsDeviceStartupProcessPerformance](intune-userExperienceAnalyticsDeviceStartupProcessPerformance.md)            | Update the properties of a userExperienceAnalyticsDeviceStartupProcessPerformance object.             |
| [Delete userExperienceAnalyticsDeviceStartupProcessPerformance](../api/intune-userexperienceanalyticsdevicestartupprocessperformance-delete.md) |                                                                                                                                       | Delete a userExperienceAnalyticsDeviceStartupProcessPerformance object.                               |

## Properties

| Property         | Type   | Description                                                                                           |
| :--------------- | :----- | :---------------------------------------------------------------------------------------------------- |
| deviceCount      | Int64  | User experience analytics device startup process summarized count.                                    |
| id               | String | The unique identifier of the user experience analytics device startup process performance. Read-only. |
| medianImpactInMs | Int32  | User experience analytics device startup process median impact in milliseconds.                       |
| processName      | String | User experience analytics device startup process name.                                                |
| productName      | String | The user experience analytics device startup process product name.                                    |
| publisher        | String | The User experience analytics device startup process publisher.                                       |
| totalImpactInMs  | Int32  | User experience analytics device startup process total impact in milliseconds.                        |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "deviceCount": "Int64",
  "id": "String (identifier)",
  "medianImpactInMs": "Int32",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "totalImpactInMs": "Int32"
}
```