---
title: "deviceManagementScriptUserState resource type"
description: "Contains properties for user run state of the device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScriptUserState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for user run state of the device management script.

## Methods

| Method                                                                                            | Return Type                                                                             | Description                                                                           |
| :------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------ |
| [List deviceManagementScriptUserState](../api/intune-devicemanagementscriptuserstate-list.md)     | [deviceManagementScriptUserState](intune-deviceManagementScriptUserState.md) collection | List properties and relationships of a deviceManagementScriptUserState object.        |
| [Create deviceManagementScriptUserState](../api/intune-devicemanagementscriptuserstate-create.md) | [deviceManagementScriptUserState](intune-deviceManagementScriptUserState.md)            | Create a new deviceManagementScriptUserState object.                                  |
| [Get deviceManagementScriptUserState](../api/intune-devicemanagementscriptuserstate-get.md)       | [deviceManagementScriptUserState](intune-deviceManagementScriptUserState.md)            | Read properties and relationships of a deviceManagementScriptUserState object.        |
| [Update deviceManagementScriptUserState](../api/intune-devicemanagementscriptuserstate-update.md) | [deviceManagementScriptUserState](intune-deviceManagementScriptUserState.md)            | Update the properties of a deviceManagementScriptUserState object.                    |
| [Delete deviceManagementScriptUserState](../api/intune-devicemanagementscriptuserstate-delete.md) |                                                                                         | Delete a deviceManagementScriptUserState object.                                      |
| [List deviceRunStates](../api/intune-devicemanagementscriptuserstate-list-devicerunstates.md)     | deviceManagementScriptDeviceState                                                       | Get the deviceManagementScriptDeviceState from a deviceRunStates navigation property. |
| [Create deviceRunStates](../api/intune-devicemanagementscriptuserstate-post-devicerunstates.md)   | deviceManagementScriptDeviceState                                                       | Create a new deviceRunStates object.                                                  |
| [Get deviceRunStates](../api/intune-devicemanagementscriptuserstate-get-devicerunstates.md)       | deviceManagementScriptDeviceState                                                       | Read the properties and relationships of a deviceManagementScriptDeviceState object.  |
| [Update deviceRunStates](../api/intune-devicemanagementscriptuserstate-update-devicerunstates.md) | deviceManagementScriptDeviceState                                                       | Update the properties of a deviceRunStates object.                                    |
| [Delete deviceRunStates](../api/intune-devicemanagementscriptuserstate-delete-devicerunstates.md) |                                                                                         | Delete a deviceManagementScriptDeviceState object.                                    |

## Properties

| Property           | Type   | Description                                                                                   |
| :----------------- | :----- | :-------------------------------------------------------------------------------------------- |
| errorDeviceCount   | Int32  | Error device count for specific user.                                                         |
| id                 | String | Key of the device management script user state entity. This property is read-only. Read-only. |
| successDeviceCount | Int32  | Success device count for specific user.                                                       |
| userPrincipalName  | String | User principle name of specific user.                                                         |

## Relationships

| Relationship    | Type                                                                                              | Description                                                             |
| :-------------- | :------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------- |
| deviceRunStates | [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection | List of run states for this script across all devices of specific user. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "errorDeviceCount": "Int32",
  "id": "String (identifier)",
  "successDeviceCount": "Int32",
  "userPrincipalName": "String"
}
```