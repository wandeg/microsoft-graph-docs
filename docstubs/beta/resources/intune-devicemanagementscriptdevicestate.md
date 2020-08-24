---
title: "deviceManagementScriptDeviceState resource type"
description: "Contains properties for device run state of the device management script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScriptDeviceState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for device run state of the device management script.

## Methods

| Method                                                                                                | Return Type                                                                                 | Description                                                                      |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------- |
| [List deviceManagementScriptDeviceState](../api/intune-devicemanagementscriptdevicestate-list.md)     | [deviceManagementScriptDeviceState](intune-deviceManagementScriptDeviceState.md) collection | List properties and relationships of a deviceManagementScriptDeviceState object. |
| [Create deviceManagementScriptDeviceState](../api/intune-devicemanagementscriptdevicestate-create.md) | [deviceManagementScriptDeviceState](intune-deviceManagementScriptDeviceState.md)            | Create a new deviceManagementScriptDeviceState object.                           |
| [Get deviceManagementScriptDeviceState](../api/intune-devicemanagementscriptdevicestate-get.md)       | [deviceManagementScriptDeviceState](intune-deviceManagementScriptDeviceState.md)            | Read properties and relationships of a deviceManagementScriptDeviceState object. |
| [Update deviceManagementScriptDeviceState](../api/intune-devicemanagementscriptdevicestate-update.md) | [deviceManagementScriptDeviceState](intune-deviceManagementScriptDeviceState.md)            | Update the properties of a deviceManagementScriptDeviceState object.             |
| [Delete deviceManagementScriptDeviceState](../api/intune-devicemanagementscriptdevicestate-delete.md) |                                                                                             | Delete a deviceManagementScriptDeviceState object.                               |
| [List managedDevice](../api/intune-devicemanagementscriptdevicestate-list-manageddevice.md)           | managedDevice                                                                               | Get the managedDevice from a managedDevice navigation property.                  |
| [Add managedDevice](../api/intune-devicemanagementscriptdevicestate-post-manageddevice.md)            | managedDevice                                                                               | Add managedDevice by posting to the managedDevice collection.                    |
| [Get managedDevice](../api/intune-devicemanagementscriptdevicestate-get-manageddevice.md)             | managedDevice                                                                               | Read the properties and relationships of a managedDevice object.                 |
| [Update managedDevice](../api/intune-devicemanagementscriptdevicestate-update-manageddevice.md)       | managedDevice                                                                               | Update the properties of a managedDevice object.                                 |
| [Remove managedDevice](../api/intune-devicemanagementscriptdevicestate-delete-manageddevice.md)       |                                                                                             | Remove a managedDevice object.                                                   |

## Properties

| Property                | Type           | Description                                                                                     |
| :---------------------- | :------------- | :---------------------------------------------------------------------------------------------- |
| errorCode               | Int32          | Error code corresponding to erroneous execution of the device management script.                |
| errorDescription        | String         | Error description corresponding to erroneous execution of the device management script.         |
| id                      | String         | Key of the device management script device state entity. This property is read-only. Read-only. |
| lastStateUpdateDateTime | DateTimeOffset | Latest time the device management script executes.                                              |
| resultMessage           | String         | Details of execution output.                                                                    |
| runState                | String         | State of latest run of the device management script.                                            |

## Relationships

| Relationship  | Type                                           | Description                                                     |
| :------------ | :--------------------------------------------- | :-------------------------------------------------------------- |
| managedDevice | [managedDevice](../resources/manageddevice.md) | The managed devices that executes the device management script. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "errorCode": "Int32",
  "errorDescription": "String",
  "id": "String (identifier)",
  "lastStateUpdateDateTime": "DateTimeOffset",
  "resultMessage": "String",
  "runState": "unknown | success | fail | scriptError | pending | notApplicable"
}
```