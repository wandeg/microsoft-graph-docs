---
title: "deviceShellScript resource type"
description: "Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceShellScript resource type


Namespace: microsoft.graph

Intune will provide customer the ability to run their Shell scripts on the enrolled Mac OS devices. The script can be run once or periodically.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceShellScript](../api/deviceshellscript-get.md)|[deviceShellScript](../resources/deviceshellscript.md)|Read properties and relationships of the [deviceShellScript](../resources/deviceshellscript.md) object.|
|[Update deviceShellScript](../api/deviceshellscript-update.md)|[deviceShellScript](../resources/deviceshellscript.md)|Update the properties of a [deviceShellScript](../resources/deviceshellscript.md) object.|
|[List groupAssignments](../api/deviceshellscript-list-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection|Get the deviceManagementScriptGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/deviceshellscript-post-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/deviceshellscript-list-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|Get the deviceManagementScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/deviceshellscript-post-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceManagementScriptRunSummary](../api/devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|
|[List deviceRunStates](../api/deviceshellscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/deviceshellscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|
|[List userRunStates](../api/deviceshellscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Add userRunStates](../api/deviceshellscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Add userRunStates by posting to the userRunStates collection.|

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

