---
title: "deviceManagementScript resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScript resource type


Namespace: microsoft.graph




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
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|enforceSignatureCheck|Boolean||
|fileName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|runAs32Bit|Boolean||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|scriptContent|Binary||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection||
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection||
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/devicemanagementscriptgroupassignment.md) collection||
|runSummary|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)||
|userRunStates|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection||

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

