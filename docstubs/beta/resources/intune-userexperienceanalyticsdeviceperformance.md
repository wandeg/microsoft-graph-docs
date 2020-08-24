---
title: "userExperienceAnalyticsDevicePerformance resource type"
description: "The user experience analytics device performance entity contains device boot performance details."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsDevicePerformance resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics device performance entity contains device boot performance details.

## Methods

| Method                                                                                                                           | Return Type                                                                                               | Description                                                                             |
| :------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsDevicePerformance](../api/intune-userexperienceanalyticsdeviceperformance-list.md)                  | [userExperienceAnalyticsDevicePerformance](intune-userExperienceAnalyticsDevicePerformance.md) collection | List properties and relationships of a userExperienceAnalyticsDevicePerformance object. |
| [Create userExperienceAnalyticsDevicePerformance](../api/intune-userexperienceanalyticsdeviceperformance-create.md)              | [userExperienceAnalyticsDevicePerformance](intune-userExperienceAnalyticsDevicePerformance.md)            | Create a new userExperienceAnalyticsDevicePerformance object.                           |
| [Get userExperienceAnalyticsDevicePerformance](../api/intune-userexperienceanalyticsdeviceperformance-get.md)                    | [userExperienceAnalyticsDevicePerformance](intune-userExperienceAnalyticsDevicePerformance.md)            | Read properties and relationships of a userExperienceAnalyticsDevicePerformance object. |
| [Update userExperienceAnalyticsDevicePerformance](../api/intune-userexperienceanalyticsdeviceperformance-update.md)              | [userExperienceAnalyticsDevicePerformance](intune-userExperienceAnalyticsDevicePerformance.md)            | Update the properties of a userExperienceAnalyticsDevicePerformance object.             |
| [Delete userExperienceAnalyticsDevicePerformance](../api/intune-userexperienceanalyticsdeviceperformance-delete.md)              |                                                                                                           | Delete a userExperienceAnalyticsDevicePerformance object.                               |
| [summarizeDevicePerformanceDevices](../api/intune-userexperienceanalyticsdeviceperformance-summarizeDevicePerformanceDevices.md) |                                                                                                           |                                                                                         |

## Properties

| Property                  | Type   | Description                                                                                       |
| :------------------------ | :----- | :------------------------------------------------------------------------------------------------ |
| bootScore                 | Int32  | The user experience analytics device boot score.                                                  |
| coreBootTimeInMs          | Int32  | The user experience analytics device core boot time in milliseconds.                              |
| coreLoginTimeInMs         | Int32  | The user experience analytics device core login time in milliseconds.                             |
| deviceCount               | Int64  | User experience analytics summarized device count.                                                |
| deviceName                | String | The user experience analytics device name.                                                        |
| diskType                  | String | The user experience analytics device disk type.                                                   |
| groupPolicyBootTimeInMs   | Int32  | The user experience analytics device group policy boot time in milliseconds.                      |
| groupPolicyLoginTimeInMs  | Int32  | The user experience analytics device group policy login time in milliseconds.                     |
| healthStatus              | String | The health state of the user experience analytics device.                                         |
| id                        | String | The unique identifier of the user experience analytics device boot performance device. Read-only. |
| loginScore                | Int32  | The user experience analytics device login score.                                                 |
| manufacturer              | String | The user experience analytics device manufacturer.                                                |
| model                     | String | The user experience analytics device model.                                                       |
| operatingSystemVersion    | String | The user experience analytics device Operating System version.                                    |
| responsiveDesktopTimeInMs | Int32  | The user experience analytics responsive desktop time in milliseconds.                            |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "bootScore": "Int32",
  "coreBootTimeInMs": "Int32",
  "coreLoginTimeInMs": "Int32",
  "deviceCount": "Int64",
  "deviceName": "String",
  "diskType": "unkown | hdd | ssd",
  "groupPolicyBootTimeInMs": "Int32",
  "groupPolicyLoginTimeInMs": "Int32",
  "healthStatus": "unknown | insufficientData | needsAttention | meetingGoals",
  "id": "String (identifier)",
  "loginScore": "Int32",
  "manufacturer": "String",
  "model": "String",
  "operatingSystemVersion": "String",
  "responsiveDesktopTimeInMs": "Int32"
}
```