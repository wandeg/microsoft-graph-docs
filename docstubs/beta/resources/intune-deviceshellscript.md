---
title: "deviceShellScript resource type"
description: "Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceShellScript resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically.

## Methods

| Method                                                                                | Return Type                                                 | Description                                                                                |
| :------------------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------- |
| [List deviceShellScript](../api/intune-deviceshellscript-list.md)                     | [deviceShellScript](intune-deviceShellScript.md) collection | List properties and relationships of a deviceShellScript object.                           |
| [Create deviceShellScript](../api/intune-deviceshellscript-create.md)                 | [deviceShellScript](intune-deviceShellScript.md)            | Create a new deviceShellScript object.                                                     |
| [Get deviceShellScript](../api/intune-deviceshellscript-get.md)                       | [deviceShellScript](intune-deviceShellScript.md)            | Read properties and relationships of a deviceShellScript object.                           |
| [Update deviceShellScript](../api/intune-deviceshellscript-update.md)                 | [deviceShellScript](intune-deviceShellScript.md)            | Update the properties of a deviceShellScript object.                                       |
| [Delete deviceShellScript](../api/intune-deviceshellscript-delete.md)                 |                                                             | Delete a deviceShellScript object.                                                         |
| [assign](../api/intune-deviceshellscript-assign.md)                                   |                                                             |                                                                                            |
| [List assignments](../api/intune-deviceshellscript-list-assignments.md)               | deviceManagementScriptAssignment                            | Get the deviceManagementScriptAssignment from an assignments navigation property.          |
| [Create assignments](../api/intune-deviceshellscript-post-assignments.md)             | deviceManagementScriptAssignment                            | Create a new assignments object.                                                           |
| [Get assignments](../api/intune-deviceshellscript-get-assignments.md)                 | deviceManagementScriptAssignment                            | Read the properties and relationships of a deviceManagementScriptAssignment object.        |
| [Update assignments](../api/intune-deviceshellscript-update-assignments.md)           | deviceManagementScriptAssignment                            | Update the properties of an assignments object.                                            |
| [Delete assignments](../api/intune-deviceshellscript-delete-assignments.md)           |                                                             | Delete a deviceManagementScriptAssignment object.                                          |
| [List deviceRunStates](../api/intune-deviceshellscript-list-devicerunstates.md)       | deviceManagementScriptDeviceState                           | Get the deviceManagementScriptDeviceState from a deviceRunStates navigation property.      |
| [Create deviceRunStates](../api/intune-deviceshellscript-post-devicerunstates.md)     | deviceManagementScriptDeviceState                           | Create a new deviceRunStates object.                                                       |
| [Get deviceRunStates](../api/intune-deviceshellscript-get-devicerunstates.md)         | deviceManagementScriptDeviceState                           | Read the properties and relationships of a deviceManagementScriptDeviceState object.       |
| [Update deviceRunStates](../api/intune-deviceshellscript-update-devicerunstates.md)   | deviceManagementScriptDeviceState                           | Update the properties of a deviceRunStates object.                                         |
| [Delete deviceRunStates](../api/intune-deviceshellscript-delete-devicerunstates.md)   |                                                             | Delete a deviceManagementScriptDeviceState object.                                         |
| [List groupAssignments](../api/intune-deviceshellscript-list-groupassignments.md)     | deviceManagementScriptGroupAssignment                       | Get the deviceManagementScriptGroupAssignment from a groupAssignments navigation property. |
| [Create groupAssignments](../api/intune-deviceshellscript-post-groupassignments.md)   | deviceManagementScriptGroupAssignment                       | Create a new groupAssignments object.                                                      |
| [Get groupAssignments](../api/intune-deviceshellscript-get-groupassignments.md)       | deviceManagementScriptGroupAssignment                       | Read the properties and relationships of a deviceManagementScriptGroupAssignment object.   |
| [Update groupAssignments](../api/intune-deviceshellscript-update-groupassignments.md) | deviceManagementScriptGroupAssignment                       | Update the properties of a groupAssignments object.                                        |
| [Delete groupAssignments](../api/intune-deviceshellscript-delete-groupassignments.md) |                                                             | Delete a deviceManagementScriptGroupAssignment object.                                     |
| [List runSummary](../api/intune-deviceshellscript-list-runsummary.md)                 | deviceManagementScriptRunSummary                            | Get the deviceManagementScriptRunSummary from a runSummary navigation property.            |
| [Add runSummary](../api/intune-deviceshellscript-post-runsummary.md)                  | deviceManagementScriptRunSummary                            | Add runSummary by posting to the runSummary collection.                                    |
| [Get runSummary](../api/intune-deviceshellscript-get-runsummary.md)                   | deviceManagementScriptRunSummary                            | Read the properties and relationships of a deviceManagementScriptRunSummary object.        |
| [Update runSummary](../api/intune-deviceshellscript-update-runsummary.md)             | deviceManagementScriptRunSummary                            | Update the properties of a runSummary object.                                              |
| [Remove runSummary](../api/intune-deviceshellscript-delete-runsummary.md)             |                                                             | Remove a deviceManagementScriptRunSummary object.                                          |
| [List userRunStates](../api/intune-deviceshellscript-list-userrunstates.md)           | deviceManagementScriptUserState                             | Get the deviceManagementScriptUserState from a userRunStates navigation property.          |
| [Create userRunStates](../api/intune-deviceshellscript-post-userrunstates.md)         | deviceManagementScriptUserState                             | Create a new userRunStates object.                                                         |
| [Get userRunStates](../api/intune-deviceshellscript-get-userrunstates.md)             | deviceManagementScriptUserState                             | Read the properties and relationships of a deviceManagementScriptUserState object.         |
| [Update userRunStates](../api/intune-deviceshellscript-update-userrunstates.md)       | deviceManagementScriptUserState                             | Update the properties of a userRunStates object.                                           |
| [Delete userRunStates](../api/intune-deviceshellscript-delete-userrunstates.md)       |                                                             | Delete a deviceManagementScriptUserState object.                                           |

## Properties

| Property                    | Type              | Description                                                                                   |
| :-------------------------- | :---------------- | :-------------------------------------------------------------------------------------------- |
| blockExecutionNotifications | Boolean           | Does not notify the user a script is being executed                                           |
| createdDateTime             | DateTimeOffset    | The date and time the device management script was created. This property is read-only.       |
| description                 | String            | Optional description for the device management script.                                        |
| displayName                 | String            | Name of the device management script.                                                         |
| executionFrequency          | Duration          | The interval for script to run. If not defined the script will run once                       |
| fileName                    | String            | Script file name.                                                                             |
| id                          | String            | Unique Identifier for the device management script. Read-only.                                |
| lastModifiedDateTime        | DateTimeOffset    | The date and time the device management script was last modified. This property is read-only. |
| retryCount                  | Int32             | Number of times for the script to be retried if it fails                                      |
| roleScopeTagIds             | String collection | List of Scope Tag IDs for this PowerShellScript instance.                                     |
| runAsAccount                | String            | Indicates the type of execution context.                                                      |
| scriptContent               | Binary            | The script content.                                                                           |

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
  "@odata.type": "microsoft.graph.deviceShellScript",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "blockExecutionNotifications": "Boolean",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "executionFrequency": "Duration",
  "fileName": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "retryCount": "Int32",
  "roleScopeTagIds": ["String"],
  "runAsAccount": "system | user",
  "scriptContent": "Binary"
}
```