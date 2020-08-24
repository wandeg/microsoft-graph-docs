---
title: "deviceHealthScriptDeviceState resource type"
description: "Contains properties for device run state of the device health script."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceHealthScriptDeviceState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties for device run state of the device health script.

## Methods

| Method                                                                                        | Return Type                                                                         | Description                                                                  |
| :-------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- | :--------------------------------------------------------------------------- |
| [List deviceHealthScriptDeviceState](../api/intune-devicehealthscriptdevicestate-list.md)     | [deviceHealthScriptDeviceState](intune-deviceHealthScriptDeviceState.md) collection | List properties and relationships of a deviceHealthScriptDeviceState object. |
| [Create deviceHealthScriptDeviceState](../api/intune-devicehealthscriptdevicestate-create.md) | [deviceHealthScriptDeviceState](intune-deviceHealthScriptDeviceState.md)            | Create a new deviceHealthScriptDeviceState object.                           |
| [Get deviceHealthScriptDeviceState](../api/intune-devicehealthscriptdevicestate-get.md)       | [deviceHealthScriptDeviceState](intune-deviceHealthScriptDeviceState.md)            | Read properties and relationships of a deviceHealthScriptDeviceState object. |
| [Update deviceHealthScriptDeviceState](../api/intune-devicehealthscriptdevicestate-update.md) | [deviceHealthScriptDeviceState](intune-deviceHealthScriptDeviceState.md)            | Update the properties of a deviceHealthScriptDeviceState object.             |
| [Delete deviceHealthScriptDeviceState](../api/intune-devicehealthscriptdevicestate-delete.md) |                                                                                     | Delete a deviceHealthScriptDeviceState object.                               |
| [List managedDevice](../api/intune-devicehealthscriptdevicestate-list-manageddevice.md)       | managedDevice                                                                       | Get the managedDevice from a managedDevice navigation property.              |
| [Add managedDevice](../api/intune-devicehealthscriptdevicestate-post-manageddevice.md)        | managedDevice                                                                       | Add managedDevice by posting to the managedDevice collection.                |
| [Get managedDevice](../api/intune-devicehealthscriptdevicestate-get-manageddevice.md)         | managedDevice                                                                       | Read the properties and relationships of a managedDevice object.             |
| [Update managedDevice](../api/intune-devicehealthscriptdevicestate-update-manageddevice.md)   | managedDevice                                                                       | Update the properties of a managedDevice object.                             |
| [Remove managedDevice](../api/intune-devicehealthscriptdevicestate-delete-manageddevice.md)   |                                                                                     | Remove a managedDevice object.                                               |

## Properties

| Property                             | Type           | Description                                                                                 |
| :----------------------------------- | :------------- | :------------------------------------------------------------------------------------------ |
| detectionState                       | String         | Detection state from the lastest device health script execution                             |
| expectedStateUpdateDateTime          | DateTimeOffset | The next timestamp of when the device health script is expected to execute                  |
| id                                   | String         | Key of the device health script device state entity. This property is read-only. Read-only. |
| lastStateUpdateDateTime              | DateTimeOffset | The last timestamp of when the device health script executed                                |
| lastSyncDateTime                     | DateTimeOffset | The last time that Intune Managment Extension synced with Intune                            |
| postRemediationDetectionScriptError  | String         | Error from the detection script after remediation                                           |
| postRemediationDetectionScriptOutput | String         | Detection script output after remediation                                                   |
| preRemediationDetectionScriptError   | String         | Error from the detection script before remediation                                          |
| preRemediationDetectionScriptOutput  | String         | Output of the detection script before remediation                                           |
| remediationScriptError               | String         | Error output of the remediation script                                                      |
| remediationState                     | String         | Remediation state from the lastest device health script execution                           |

## Relationships

| Relationship  | Type                                           | Description                                                   |
| :------------ | :--------------------------------------------- | :------------------------------------------------------------ |
| managedDevice | [managedDevice](../resources/manageddevice.md) | The managed device on which the device health script executed |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "unknown | success | fail | scriptError | pending | notApplicable",
  "expectedStateUpdateDateTime": "DateTimeOffset",
  "id": "String (identifier)",
  "lastStateUpdateDateTime": "DateTimeOffset",
  "lastSyncDateTime": "DateTimeOffset",
  "postRemediationDetectionScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "preRemediationDetectionScriptOutput": "String",
  "remediationScriptError": "String",
  "remediationState": "unknown | skipped | success | remediationFailed | scriptError"
}
```