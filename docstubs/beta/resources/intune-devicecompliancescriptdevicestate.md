---
title: "deviceComplianceScriptDeviceState resource type"
description: "Contains properties for device run state of the device compliance script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceComplianceScriptDeviceState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for device run state of the device compliance script.

## Methods

| Method                                                                                                | Return Type                                                                                 | Description                                                                      |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------- |
| [List deviceComplianceScriptDeviceState](../api/intune-devicecompliancescriptdevicestate-list.md)     | [deviceComplianceScriptDeviceState](intune-deviceComplianceScriptDeviceState.md) collection | List properties and relationships of a deviceComplianceScriptDeviceState object. |
| [Create deviceComplianceScriptDeviceState](../api/intune-devicecompliancescriptdevicestate-create.md) | [deviceComplianceScriptDeviceState](intune-deviceComplianceScriptDeviceState.md)            | Create a new deviceComplianceScriptDeviceState object.                           |
| [Get deviceComplianceScriptDeviceState](../api/intune-devicecompliancescriptdevicestate-get.md)       | [deviceComplianceScriptDeviceState](intune-deviceComplianceScriptDeviceState.md)            | Read properties and relationships of a deviceComplianceScriptDeviceState object. |
| [Update deviceComplianceScriptDeviceState](../api/intune-devicecompliancescriptdevicestate-update.md) | [deviceComplianceScriptDeviceState](intune-deviceComplianceScriptDeviceState.md)            | Update the properties of a deviceComplianceScriptDeviceState object.             |
| [Delete deviceComplianceScriptDeviceState](../api/intune-devicecompliancescriptdevicestate-delete.md) |                                                                                             | Delete a deviceComplianceScriptDeviceState object.                               |
| [List managedDevice](../api/intune-devicecompliancescriptdevicestate-list-manageddevice.md)           | managedDevice                                                                               | Get the managedDevice from a managedDevice navigation property.                  |
| [Add managedDevice](../api/intune-devicecompliancescriptdevicestate-post-manageddevice.md)            | managedDevice                                                                               | Add managedDevice by posting to the managedDevice collection.                    |
| [Get managedDevice](../api/intune-devicecompliancescriptdevicestate-get-manageddevice.md)             | managedDevice                                                                               | Read the properties and relationships of a managedDevice object.                 |
| [Update managedDevice](../api/intune-devicecompliancescriptdevicestate-update-manageddevice.md)       | managedDevice                                                                               | Update the properties of a managedDevice object.                                 |
| [Remove managedDevice](../api/intune-devicecompliancescriptdevicestate-delete-manageddevice.md)       |                                                                                             | Remove a managedDevice object.                                                   |

## Properties

| Property                    | Type           | Description                                                                                     |
| :-------------------------- | :------------- | :---------------------------------------------------------------------------------------------- |
| detectionState              | String         | Detection state from the lastest device compliance script execution                             |
| expectedStateUpdateDateTime | DateTimeOffset | The next timestamp of when the device compliance script is expected to execute                  |
| id                          | String         | Key of the device compliance script device state entity. This property is read-only. Read-only. |
| lastStateUpdateDateTime     | DateTimeOffset | The last timestamp of when the device compliance script executed                                |
| lastSyncDateTime            | DateTimeOffset | The last time that Intune Managment Extension synced with Intune                                |
| scriptError                 | String         | Error from the detection script                                                                 |
| scriptOutput                | String         | Output of the detection script                                                                  |

## Relationships

| Relationship  | Type                                           | Description                                                       |
| :------------ | :--------------------------------------------- | :---------------------------------------------------------------- |
| managedDevice | [managedDevice](../resources/manageddevice.md) | The managed device on which the device compliance script executed |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
  "detectionState": "unknown | success | fail | scriptError | pending | notApplicable",
  "expectedStateUpdateDateTime": "DateTimeOffset",
  "id": "String (identifier)",
  "lastStateUpdateDateTime": "DateTimeOffset",
  "lastSyncDateTime": "DateTimeOffset",
  "scriptError": "String",
  "scriptOutput": "String"
}
```