---
title: "deviceComplianceScript resource type"
description: "Intune will provide customer the ability to run their Powershell Compliance scripts (detection) on the enrolled windows 10 Azure Active Directory joined devices."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceComplianceScript resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Intune will provide customer the ability to run their Powershell Compliance scripts (detection) on the enrolled windows 10 Azure Active Directory joined devices.

## Methods

| Method                                                                                   | Return Type                                                           | Description                                                                           |
| :--------------------------------------------------------------------------------------- | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------ |
| [List deviceComplianceScript](../api/intune-devicecompliancescript-list.md)              | [deviceComplianceScript](intune-deviceComplianceScript.md) collection | List properties and relationships of a deviceComplianceScript object.                 |
| [Create deviceComplianceScript](../api/intune-devicecompliancescript-create.md)          | [deviceComplianceScript](intune-deviceComplianceScript.md)            | Create a new deviceComplianceScript object.                                           |
| [Get deviceComplianceScript](../api/intune-devicecompliancescript-get.md)                | [deviceComplianceScript](intune-deviceComplianceScript.md)            | Read properties and relationships of a deviceComplianceScript object.                 |
| [Update deviceComplianceScript](../api/intune-devicecompliancescript-update.md)          | [deviceComplianceScript](intune-deviceComplianceScript.md)            | Update the properties of a deviceComplianceScript object.                             |
| [Delete deviceComplianceScript](../api/intune-devicecompliancescript-delete.md)          |                                                                       | Delete a deviceComplianceScript object.                                               |
| [assign](../api/intune-devicecompliancescript-assign.md)                                 |                                                                       |                                                                                       |
| [List assignments](../api/intune-devicecompliancescript-list-assignments.md)             | deviceHealthScriptAssignment                                          | Get the deviceHealthScriptAssignment from an assignments navigation property.         |
| [Create assignments](../api/intune-devicecompliancescript-post-assignments.md)           | deviceHealthScriptAssignment                                          | Create a new assignments object.                                                      |
| [Get assignments](../api/intune-devicecompliancescript-get-assignments.md)               | deviceHealthScriptAssignment                                          | Read the properties and relationships of a deviceHealthScriptAssignment object.       |
| [Update assignments](../api/intune-devicecompliancescript-update-assignments.md)         | deviceHealthScriptAssignment                                          | Update the properties of an assignments object.                                       |
| [Delete assignments](../api/intune-devicecompliancescript-delete-assignments.md)         |                                                                       | Delete a deviceHealthScriptAssignment object.                                         |
| [List deviceRunStates](../api/intune-devicecompliancescript-list-devicerunstates.md)     | deviceComplianceScriptDeviceState                                     | Get the deviceComplianceScriptDeviceState from a deviceRunStates navigation property. |
| [Create deviceRunStates](../api/intune-devicecompliancescript-post-devicerunstates.md)   | deviceComplianceScriptDeviceState                                     | Create a new deviceRunStates object.                                                  |
| [Get deviceRunStates](../api/intune-devicecompliancescript-get-devicerunstates.md)       | deviceComplianceScriptDeviceState                                     | Read the properties and relationships of a deviceComplianceScriptDeviceState object.  |
| [Update deviceRunStates](../api/intune-devicecompliancescript-update-devicerunstates.md) | deviceComplianceScriptDeviceState                                     | Update the properties of a deviceRunStates object.                                    |
| [Delete deviceRunStates](../api/intune-devicecompliancescript-delete-devicerunstates.md) |                                                                       | Delete a deviceComplianceScriptDeviceState object.                                    |
| [List runSummary](../api/intune-devicecompliancescript-list-runsummary.md)               | deviceComplianceScriptRunSummary                                      | Get the deviceComplianceScriptRunSummary from a runSummary navigation property.       |
| [Create runSummary](../api/intune-devicecompliancescript-post-runsummary.md)             | deviceComplianceScriptRunSummary                                      | Create a new runSummary object.                                                       |
| [Get runSummary](../api/intune-devicecompliancescript-get-runsummary.md)                 | deviceComplianceScriptRunSummary                                      | Read the properties and relationships of a deviceComplianceScriptRunSummary object.   |
| [Update runSummary](../api/intune-devicecompliancescript-update-runsummary.md)           | deviceComplianceScriptRunSummary                                      | Update the properties of a runSummary object.                                         |
| [Delete runSummary](../api/intune-devicecompliancescript-delete-runsummary.md)           |                                                                       | Delete a deviceComplianceScriptRunSummary object.                                     |

## Properties

| Property               | Type              | Description                                                                                  |
| :--------------------- | :---------------- | :------------------------------------------------------------------------------------------- |
| createdDateTime        | DateTimeOffset    | The timestamp of when the device compliance script was created. This property is read-only.  |
| description            | String            | Description of the device compliance script                                                  |
| detectionScriptContent | Binary            | The entire content of the detection powershell script                                        |
| displayName            | String            | Name of the device compliance script                                                         |
| enforceSignatureCheck  | Boolean           | Indicate whether the script signature needs be checked                                       |
| id                     | String            | Unique Identifier for the device compliance script Read-only.                                |
| lastModifiedDateTime   | DateTimeOffset    | The timestamp of when the device compliance script was modified. This property is read-only. |
| publisher              | String            | Name of the device compliance script publisher                                               |
| roleScopeTagIds        | String collection | List of Scope Tag IDs for the device compliance script                                       |
| runAs32Bit             | Boolean           | Indicate whether PowerShell script(s) should run as 32-bit                                   |
| runAsAccount           | String            | Indicates the type of execution context                                                      |
| version                | String            | Version of the device compliance script                                                      |

## Relationships

| Relationship    | Type                                                                                              | Description                                                            |
| :-------------- | :------------------------------------------------------------------------------------------------ | :--------------------------------------------------------------------- |
| assignments     | [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection           | The list of group assignments for the device compliance script         |
| deviceRunStates | [deviceComplianceScriptDeviceState](../resources/devicecompliancescriptdevicestate.md) collection | List of run states for the device compliance script across all devices |
| runSummary      | [deviceComplianceScriptRunSummary](../resources/devicecompliancescriptrunsummary.md)              | High level run summary for device compliance script.                   |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "detectionScriptContent": "Binary",
  "displayName": "String",
  "enforceSignatureCheck": "Boolean",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "publisher": "String",
  "roleScopeTagIds": ["String"],
  "runAs32Bit": "Boolean",
  "runAsAccount": "system | user",
  "version": "String"
}
```