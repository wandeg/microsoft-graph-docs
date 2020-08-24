---
title: "deviceManagementScript resource type"
description: "Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices. The script can be run once or periodically."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceManagementScript resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices. The script can be run once or periodically.

## Methods

| Method                                                                                     | Return Type                                                           | Description                                                                                |
| :----------------------------------------------------------------------------------------- | :-------------------------------------------------------------------- | :----------------------------------------------------------------------------------------- |
| [List deviceManagementScript](../api/intune-devicemanagementscript-list.md)                | [deviceManagementScript](intune-deviceManagementScript.md) collection | List properties and relationships of a deviceManagementScript object.                      |
| [Create deviceManagementScript](../api/intune-devicemanagementscript-create.md)            | [deviceManagementScript](intune-deviceManagementScript.md)            | Create a new deviceManagementScript object.                                                |
| [Get deviceManagementScript](../api/intune-devicemanagementscript-get.md)                  | [deviceManagementScript](intune-deviceManagementScript.md)            | Read properties and relationships of a deviceManagementScript object.                      |
| [Update deviceManagementScript](../api/intune-devicemanagementscript-update.md)            | [deviceManagementScript](intune-deviceManagementScript.md)            | Update the properties of a deviceManagementScript object.                                  |
| [Delete deviceManagementScript](../api/intune-devicemanagementscript-delete.md)            |                                                                       | Delete a deviceManagementScript object.                                                    |
| [assign](../api/intune-devicemanagementscript-assign.md)                                   |                                                                       |                                                                                            |
| [List assignments](../api/intune-devicemanagementscript-list-assignments.md)               | deviceManagementScriptAssignment                                      | Get the deviceManagementScriptAssignment from an assignments navigation property.          |
| [Create assignments](../api/intune-devicemanagementscript-post-assignments.md)             | deviceManagementScriptAssignment                                      | Create a new assignments object.                                                           |
| [Get assignments](../api/intune-devicemanagementscript-get-assignments.md)                 | deviceManagementScriptAssignment                                      | Read the properties and relationships of a deviceManagementScriptAssignment object.        |
| [Update assignments](../api/intune-devicemanagementscript-update-assignments.md)           | deviceManagementScriptAssignment                                      | Update the properties of an assignments object.                                            |
| [Delete assignments](../api/intune-devicemanagementscript-delete-assignments.md)           |                                                                       | Delete a deviceManagementScriptAssignment object.                                          |
| [List deviceRunStates](../api/intune-devicemanagementscript-list-devicerunstates.md)       | deviceManagementScriptDeviceState                                     | Get the deviceManagementScriptDeviceState from a deviceRunStates navigation property.      |
| [Create deviceRunStates](../api/intune-devicemanagementscript-post-devicerunstates.md)     | deviceManagementScriptDeviceState                                     | Create a new deviceRunStates object.                                                       |
| [Get deviceRunStates](../api/intune-devicemanagementscript-get-devicerunstates.md)         | deviceManagementScriptDeviceState                                     | Read the properties and relationships of a deviceManagementScriptDeviceState object.       |
| [Update deviceRunStates](../api/intune-devicemanagementscript-update-devicerunstates.md)   | deviceManagementScriptDeviceState                                     | Update the properties of a deviceRunStates object.                                         |
| [Delete deviceRunStates](../api/intune-devicemanagementscript-delete-devicerunstates.md)   |                                                                       | Delete a deviceManagementScriptDeviceState object.                                         |
| [List groupAssignments](../api/intune-devicemanagementscript-list-groupassignments.md)     | deviceManagementScriptGroupAssignment                                 | Get the deviceManagementScriptGroupAssignment from a groupAssignments navigation property. |
| [Create groupAssignments](../api/intune-devicemanagementscript-post-groupassignments.md)   | deviceManagementScriptGroupAssignment                                 | Create a new groupAssignments object.                                                      |
| [Get groupAssignments](../api/intune-devicemanagementscript-get-groupassignments.md)       | deviceManagementScriptGroupAssignment                                 | Read the properties and relationships of a deviceManagementScriptGroupAssignment object.   |
| [Update groupAssignments](../api/intune-devicemanagementscript-update-groupassignments.md) | deviceManagementScriptGroupAssignment                                 | Update the properties of a groupAssignments object.                                        |
| [Delete groupAssignments](../api/intune-devicemanagementscript-delete-groupassignments.md) |                                                                       | Delete a deviceManagementScriptGroupAssignment object.                                     |
| [List runSummary](../api/intune-devicemanagementscript-list-runsummary.md)                 | deviceManagementScriptRunSummary                                      | Get the deviceManagementScriptRunSummary from a runSummary navigation property.            |
| [Add runSummary](../api/intune-devicemanagementscript-post-runsummary.md)                  | deviceManagementScriptRunSummary                                      | Add runSummary by posting to the runSummary collection.                                    |
| [Get runSummary](../api/intune-devicemanagementscript-get-runsummary.md)                   | deviceManagementScriptRunSummary                                      | Read the properties and relationships of a deviceManagementScriptRunSummary object.        |
| [Update runSummary](../api/intune-devicemanagementscript-update-runsummary.md)             | deviceManagementScriptRunSummary                                      | Update the properties of a runSummary object.                                              |
| [Remove runSummary](../api/intune-devicemanagementscript-delete-runsummary.md)             |                                                                       | Remove a deviceManagementScriptRunSummary object.                                          |
| [List userRunStates](../api/intune-devicemanagementscript-list-userrunstates.md)           | deviceManagementScriptUserState                                       | Get the deviceManagementScriptUserState from a userRunStates navigation property.          |
| [Create userRunStates](../api/intune-devicemanagementscript-post-userrunstates.md)         | deviceManagementScriptUserState                                       | Create a new userRunStates object.                                                         |
| [Get userRunStates](../api/intune-devicemanagementscript-get-userrunstates.md)             | deviceManagementScriptUserState                                       | Read the properties and relationships of a deviceManagementScriptUserState object.         |
| [Update userRunStates](../api/intune-devicemanagementscript-update-userrunstates.md)       | deviceManagementScriptUserState                                       | Update the properties of a userRunStates object.                                           |
| [Delete userRunStates](../api/intune-devicemanagementscript-delete-userrunstates.md)       |                                                                       | Delete a deviceManagementScriptUserState object.                                           |

## Properties

| Property              | Type              | Description                                                                                   |
| :-------------------- | :---------------- | :-------------------------------------------------------------------------------------------- |
| createdDateTime       | DateTimeOffset    | The date and time the device management script was created. This property is read-only.       |
| description           | String            | Optional description for the device management script.                                        |
| displayName           | String            | Name of the device management script.                                                         |
| enforceSignatureCheck | Boolean           | Indicate whether the script signature needs be checked.                                       |
| fileName              | String            | Script file name.                                                                             |
| id                    | String            | Unique Identifier for the device management script. Read-only.                                |
| lastModifiedDateTime  | DateTimeOffset    | The date and time the device management script was last modified. This property is read-only. |
| roleScopeTagIds       | String collection | List of Scope Tag IDs for this PowerShellScript instance.                                     |
| runAs32Bit            | Boolean           | A value indicating whether the PowerShell script should run as 32-bit                         |
| runAsAccount          | String            | Indicates the type of execution context.                                                      |
| scriptContent         | Binary            | The script content.                                                                           |

## Relationships

| Relationship     | Type                                                                                                      | Description                                                     |
| :--------------- | :-------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| assignments      | [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection           | The list of group assignments for the device management script. |
| deviceRunStates  | [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection         | List of run states for this script across all devices.          |
| groupAssignments | [deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection | The list of group assignments for the device management script. |
| runSummary       | [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)                      | Run summary for device management script.                       |
| userRunStates    | [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection             | List of run states for this script across all users.            |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "enforceSignatureCheck": "Boolean",
  "fileName": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "roleScopeTagIds": ["String"],
  "runAs32Bit": "Boolean",
  "runAsAccount": "system | user",
  "scriptContent": "Binary"
}
```