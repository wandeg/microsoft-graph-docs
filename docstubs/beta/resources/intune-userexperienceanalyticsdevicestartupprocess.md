---
title: "userExperienceAnalyticsDeviceStartupProcess resource type"
description: "The user experience analytics device startup process details."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# userExperienceAnalyticsDeviceStartupProcess resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics device startup process details.

## Methods

| Method                                                                                                                    | Return Type                                                                                                     | Description                                                                                |
| :------------------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------- |
| [List userExperienceAnalyticsDeviceStartupProcess](../api/intune-userexperienceanalyticsdevicestartupprocess-list.md)     | [userExperienceAnalyticsDeviceStartupProcess](intune-userExperienceAnalyticsDeviceStartupProcess.md) collection | List properties and relationships of a userExperienceAnalyticsDeviceStartupProcess object. |
| [Create userExperienceAnalyticsDeviceStartupProcess](../api/intune-userexperienceanalyticsdevicestartupprocess-create.md) | [userExperienceAnalyticsDeviceStartupProcess](intune-userExperienceAnalyticsDeviceStartupProcess.md)            | Create a new userExperienceAnalyticsDeviceStartupProcess object.                           |
| [Get userExperienceAnalyticsDeviceStartupProcess](../api/intune-userexperienceanalyticsdevicestartupprocess-get.md)       | [userExperienceAnalyticsDeviceStartupProcess](intune-userExperienceAnalyticsDeviceStartupProcess.md)            | Read properties and relationships of a userExperienceAnalyticsDeviceStartupProcess object. |
| [Update userExperienceAnalyticsDeviceStartupProcess](../api/intune-userexperienceanalyticsdevicestartupprocess-update.md) | [userExperienceAnalyticsDeviceStartupProcess](intune-userExperienceAnalyticsDeviceStartupProcess.md)            | Update the properties of a userExperienceAnalyticsDeviceStartupProcess object.             |
| [Delete userExperienceAnalyticsDeviceStartupProcess](../api/intune-userexperienceanalyticsdevicestartupprocess-delete.md) |                                                                                                                 | Delete a userExperienceAnalyticsDeviceStartupProcess object.                               |

## Properties

| Property          | Type   | Description                                                                               |
| :---------------- | :----- | :---------------------------------------------------------------------------------------- |
| id                | String | The unique identifier of the user experience analytics device startup process. Read-only. |
| managedDeviceId   | String | The user experience analytics device id.                                                  |
| processName       | String | User experience analytics device startup process name.                                    |
| productName       | String | The user experience analytics device startup process product name.                        |
| publisher         | String | The User experience analytics device startup process publisher.                           |
| startupImpactInMs | Int32  | User experience analytics device startup process impact in milliseconds.                  |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": "Int32"
}
```