---
title: "deviceShellScript resource type"
description: "Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceShellScript resource type


Namespace: microsoft.graph

Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceShellScript](../api/deviceshellscript-get.md)|[deviceShellScript](../resources/deviceshellscript.md)|Read the properties and relationships of a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[Update deviceShellScript](../api/deviceshellscript-update.md)|[deviceShellScript](../resources/deviceshellscript.md)|Update the properties of a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[assign](../api/deviceshellscript-assign.md)|None|**TODO: Add Description**|
|[List groupAssignments](../api/deviceshellscript-list-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection|Get the deviceManagementScriptGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/deviceshellscript-post-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md)|Create a new groupAssignments object.|
|[Delete groupAssignments](../api/deviceshellscript-delete-groupassignments.md)|None|Delete a [deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) object.|
|[Update groupAssignments](../api/deviceshellscript-update-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md)|Update the properties of a groupAssignments object.|
|[Get deviceManagementScriptGroupAssignment](../api/devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md)|Read the properties and relationships of a [deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) object.|
|[List assignments](../api/deviceshellscript-list-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|Get the deviceManagementScriptAssignments from the assignments navigation property.|
|[Create assignments](../api/deviceshellscript-post-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/deviceshellscript-delete-assignments.md)|None|Delete an [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[Update assignments](../api/deviceshellscript-update-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Update the properties of an assignments object.|
|[Get deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Read the properties and relationships of a [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[List runSummary](../api/deviceshellscript-list-runsummary.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) collection|Get the deviceManagementScriptRunSummaries from the runSummary navigation property.|
|[Add runSummary](../api/deviceshellscript-post-runsummary.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Add runSummary by posting to the runSummary collection.|
|[Remove runSummary](../api/deviceshellscript-delete-runsummary.md)|None|Remove a [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|
|[List deviceRunStates](../api/deviceshellscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Create deviceRunStates](../api/deviceshellscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Create a new deviceRunStates object.|
|[Delete deviceRunStates](../api/deviceshellscript-delete-devicerunstates.md)|None|Delete a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[Update deviceRunStates](../api/deviceshellscript-update-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Update the properties of a deviceRunStates object.|
|[Get deviceManagementScriptDeviceState](../api/devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Read the properties and relationships of a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[List userRunStates](../api/deviceshellscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Create userRunStates](../api/deviceshellscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Create a new userRunStates object.|
|[Delete userRunStates](../api/deviceshellscript-delete-userrunstates.md)|None|Delete a [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.|
|[Update userRunStates](../api/deviceshellscript-update-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Update the properties of a userRunStates object.|
|[Get deviceManagementScriptUserState](../api/devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Read the properties and relationships of a [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blockExecutionNotifications|Boolean|Does not notify the user a script is being executed|
|createdDateTime|DateTimeOffset|The date and time the device management script was created. This property is read-only.|
|description|String|Optional description for the device management script.|
|displayName|String|Name of the device management script.|
|executionFrequency|Duration|The interval for script to run. If not defined the script will run once|
|fileName|String|Script file name.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the device management script was last modified. This property is read-only.|
|retryCount|Int32|Number of times for the script to be retried if it fails|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this PowerShellScript instance.|
|runAsAccount|runAsAccountType|Indicates the type of execution context. Possible values are: `system`, `user`.|
|scriptContent|Binary|The script content.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|The list of group assignments for the device management script.|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|List of run states for this script across all devices.|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection|The list of group assignments for the device management script.|
|runSummary|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Run summary for device management script.|
|userRunStates|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|List of run states for this script across all users.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceShellScript",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "id": "String (identifier)",
  "executionFrequency": "String (duration)",
  "retryCount": 1024,
  "blockExecutionNotifications": true,
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

