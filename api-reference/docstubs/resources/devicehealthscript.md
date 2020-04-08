---
title: "deviceHealthScript resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScript resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScript](../api/devicehealthscript-get.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Read properties and relationships of the [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[Update deviceHealthScript](../api/devicehealthscript-update.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Update the properties of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[assign](../api/devicehealthscript-assign.md)|None||
|[updateGlobalScript](../api/devicehealthscript-updateglobalscript.md)|String||
|[getGlobalScriptHighestAvailableVersion](../api/devicehealthscript-getglobalscripthighestavailableversion.md)|String||
|[enableGlobalScripts](../api/devicehealthscript-enableglobalscripts.md)|None||
|[areGlobalScriptsAvailable](../api/devicehealthscript-areglobalscriptsavailable.md)|Enumeration||
|[getRemediationSummary](../api/devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/devicehealthscriptremediationsummary.md)||
|[List assignments](../api/devicehealthscript-list-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|Get the deviceHealthScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/devicehealthscript-post-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceHealthScriptRunSummary](../api/devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[List deviceRunStates](../api/devicehealthscript-list-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/devicehealthscript-post-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|detectionScriptContent|Binary||
|displayName|String||
|enforceSignatureCheck|Boolean||
|highestAvailableVersion|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isGlobalScript|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|publisher|String||
|remediationScriptContent|Binary||
|roleScopeTagIds|String collection||
|runAs32Bit|Boolean||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|version|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection||
|deviceRunStates|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection||
|runSummary|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String"
}
```

