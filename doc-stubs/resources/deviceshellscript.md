---
title: "deviceShellScript resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceShellScript resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
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
|blockExecutionNotifications|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|executionFrequency|Duration|**TODO: Add Description**|
|fileName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|retryCount|Int32|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|scriptContent|Binary|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|**TODO: Add Description**|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|**TODO: Add Description**|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection|**TODO: Add Description**|
|runSummary|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|**TODO: Add Description**|
|userRunStates|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "retryCount": "Integer",
  "blockExecutionNotifications": "Boolean",
  "displayName": "String",
  "description": "String",
  "scriptContent": "Binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

