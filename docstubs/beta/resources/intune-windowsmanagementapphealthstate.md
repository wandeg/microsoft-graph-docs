---
title: "windowsManagementAppHealthState resource type"
description: "Windows management app health state entity."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# windowsManagementAppHealthState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows management app health state entity.

## Methods

| Method                                                                                            | Return Type                                                                             | Description                                                                    |
| :------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| [List windowsManagementAppHealthState](../api/intune-windowsmanagementapphealthstate-list.md)     | [windowsManagementAppHealthState](intune-windowsManagementAppHealthState.md) collection | List properties and relationships of a windowsManagementAppHealthState object. |
| [Create windowsManagementAppHealthState](../api/intune-windowsmanagementapphealthstate-create.md) | [windowsManagementAppHealthState](intune-windowsManagementAppHealthState.md)            | Create a new windowsManagementAppHealthState object.                           |
| [Get windowsManagementAppHealthState](../api/intune-windowsmanagementapphealthstate-get.md)       | [windowsManagementAppHealthState](intune-windowsManagementAppHealthState.md)            | Read properties and relationships of a windowsManagementAppHealthState object. |
| [Update windowsManagementAppHealthState](../api/intune-windowsmanagementapphealthstate-update.md) | [windowsManagementAppHealthState](intune-windowsManagementAppHealthState.md)            | Update the properties of a windowsManagementAppHealthState object.             |
| [Delete windowsManagementAppHealthState](../api/intune-windowsmanagementapphealthstate-delete.md) |                                                                                         | Delete a windowsManagementAppHealthState object.                               |

## Properties

| Property            | Type           | Description                                                                                           |
| :------------------ | :------------- | :---------------------------------------------------------------------------------------------------- |
| deviceName          | String         | Name of the device on which Windows management app is installed.                                      |
| deviceOSVersion     | String         | Windows 10 OS version of the device on which Windows management app is installed.                     |
| healthState         | String         | Windows management app health state.                                                                  |
| id                  | String         | Unique Identifier for the Windows management app health state. This property is read-only. Read-only. |
| installedVersion    | String         | Windows management app installed version.                                                             |
| lastCheckInDateTime | DateTimeOffset | Windows management app last check-in time.                                                            |

## Relationships

| Relationship | Type | Description |
| :----------- | :--- | :---------- |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "deviceName": "String",
  "deviceOSVersion": "String",
  "healthState": "unknown | healthy | unhealthy",
  "id": "String (identifier)",
  "installedVersion": "String",
  "lastCheckInDateTime": "DateTimeOffset"
}
```