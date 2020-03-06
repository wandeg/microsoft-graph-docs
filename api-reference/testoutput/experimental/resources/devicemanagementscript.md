---
title: "deviceManagementScript resource type"
description: "Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices. The script can be run once or periodically."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScript resource type


Namespace: microsoft.graph

Intune will provide customer the ability to run their Powershell scripts on the enrolled windows 10 Azure Active Directory joined devices. The script can be run once or periodically.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementScript](../api/devicemanagementscript-get.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Read properties and relationships of the [deviceManagementScript](../resources/devicemanagementscript.md) object.|
|[Update deviceManagementScript](../api/devicemanagementscript-update.md)|[deviceManagementScript](../resources/devicemanagementscript.md)|Update the properties of a [deviceManagementScript](../resources/devicemanagementscript.md) object.|
|[hasPayloadLinks](../api/devicemanagementscript-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[assign](../api/devicemanagementscript-assign.md)|None||
|[List groupAssignments](../api/devicemanagementscript-list-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection|Get the deviceManagementScriptGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/devicemanagementscript-post-groupassignments.md)|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/devicemanagementscript-list-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|Get the deviceManagementScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/devicemanagementscript-post-assignments.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceManagementScriptRunSummary](../api/devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|
|[List deviceRunStates](../api/devicemanagementscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/devicemanagementscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|
|[List userRunStates](../api/devicemanagementscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Add userRunStates](../api/devicemanagementscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Add userRunStates by posting to the userRunStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the device management script was created. This property is read-only.|
|description|String|Optional description for the device management script.|
|displayName|String|Name of the device management script.|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked.|
|fileName|String|Script file name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the device management script was last modified. This property is read-only.|
|roleScopeTagIds|String collection|List of Scope Tag IDs for this PowerShellScript instance.|
|runAs32Bit|Boolean|A value indicating whether the PowerShell script should run as 32-bit|
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
  "@odata.type": "microsoft.graph.deviceManagementScript",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
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

