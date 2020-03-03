---
title: "deviceShellScript resource type"
description: "Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceShellScript resource type

Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md)|Read properties and relationships of the [deviceShellScript](../resources/deviceshellscript.md) object.|
|[Delete deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|None|Deletes a [deviceShellScript](../resources/deviceshellscript.md).|
|[Update deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md)|Update the properties of a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[List groupAssignments](../api/intune-devices-deviceshellscript-list-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-deviceManagementScriptGroupAssignment.md) collection|Get the deviceManagementScriptGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/intune-devices-deviceshellscript-post-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-deviceManagementScriptGroupAssignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/intune-devices-deviceshellscript-list-assignments.md)|[deviceManagementScriptAssignment](../resources/intune-devices-deviceManagementScriptAssignment.md) collection|Get the deviceManagementScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/intune-devices-deviceshellscript-post-assignments.md)|[deviceManagementScriptAssignment](../resources/intune-devices-deviceManagementScriptAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-deviceManagementScriptRunSummary.md)|Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|
|[List deviceRunStates](../api/intune-devices-deviceshellscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-deviceManagementScriptDeviceState.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/intune-devices-deviceshellscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-deviceManagementScriptDeviceState.md)|Add deviceRunStates by posting to the deviceRunStates collection.|
|[List userRunStates](../api/intune-devices-deviceshellscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/intune-devices-deviceManagementScriptUserState.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Add userRunStates](../api/intune-devices-deviceshellscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/intune-devices-deviceManagementScriptUserState.md)|Add userRunStates by posting to the userRunStates collection.|
|[List deviceShellScripts](../api/intune-devices-devicemanagement-list-deviceshellscripts.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md) collection|Get the deviceShellScripts from the deviceShellScripts navigation property.|
|[Add deviceShellScripts](../api/intune-devices-devicemanagement-post-deviceshellscripts.md)|[deviceShellScript](../resources/intune-devices-deviceShellScript.md)|Add deviceShellScripts by posting to the deviceShellScripts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the device management script was created. This property is read-only.|
|description|String|Optional description for the device management script.|
|displayName|String|Name of the device management script.|
|fileName|String|Script file name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the device management script was last modified. This property is read-only.|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this PowerShellScript instance.|
|runAsAccount|Enumeration|Indicates the type of execution context. Possible values are: `system`, `user`.|
|scriptContent|Binary|The script content.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-deviceManagementScriptAssignment.md) collection|The list of group assignments for the device management script.|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-deviceManagementScriptDeviceState.md) collection|List of run states for this script across all devices.|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-deviceManagementScriptGroupAssignment.md) collection|The list of group assignments for the device management script.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-deviceManagementScriptRunSummary.md)|Run summary for device management script.|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-deviceManagementScriptUserState.md) collection|List of run states for this script across all users.|

## JSON Representation
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

