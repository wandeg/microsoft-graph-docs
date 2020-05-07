---
title: "deviceHealthScript resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScript resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/devicehealthscript-assign.md)|None|**TODO: Add Description**|
|[updateGlobalScript](../api/devicehealthscript-updateglobalscript.md)|String|**TODO: Add Description**|
|[getGlobalScriptHighestAvailableVersion](../api/devicehealthscript-getglobalscripthighestavailableversion.md)|String|**TODO: Add Description**|
|[getRemediationHistory](../api/devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/devicehealthscriptremediationhistory.md)|**TODO: Add Description**|
|[enableGlobalScripts](../api/devicehealthscript-enableglobalscripts.md)|None|**TODO: Add Description**|
|[areGlobalScriptsAvailable](../api/devicehealthscript-areglobalscriptsavailable.md)|globalDeviceHealthScriptState|**TODO: Add Description**|
|[getRemediationSummary](../api/devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/devicehealthscriptremediationsummary.md)|**TODO: Add Description**|
|[List assignments](../api/devicehealthscript-list-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|Get the deviceHealthScriptAssignments from the assignments navigation property.|
|[Create assignments](../api/devicehealthscript-post-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/devicehealthscript-delete-assignments.md)|None|Delete an [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|
|[Update assignments](../api/devicehealthscript-update-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Update the properties of an assignments object.|
|[Get deviceHealthScriptAssignment](../api/devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Read the properties and relationships of a [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|
|[List runSummary](../api/devicehealthscript-list-runsummary.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) collection|Get the deviceHealthScriptRunSummaries from the runSummary navigation property.|
|[Create runSummary](../api/devicehealthscript-post-runsummary.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Create a new runSummary object.|
|[Delete runSummary](../api/devicehealthscript-delete-runsummary.md)|None|Delete a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[Update runSummary](../api/devicehealthscript-update-runsummary.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Update the properties of a runSummary object.|
|[Get deviceHealthScriptRunSummary](../api/devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Read the properties and relationships of a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[List deviceRunStates](../api/devicehealthscript-list-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.|
|[Create deviceRunStates](../api/devicehealthscript-post-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Create a new deviceRunStates object.|
|[Delete deviceRunStates](../api/devicehealthscript-delete-devicerunstates.md)|None|Delete a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.|
|[Update deviceRunStates](../api/devicehealthscript-update-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Update the properties of a deviceRunStates object.|
|[Get deviceHealthScriptDeviceState](../api/devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Read the properties and relationships of a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|detectionScriptContent|Binary|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|enforceSignatureCheck|Boolean|**TODO: Add Description**|
|highestAvailableVersion|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isGlobalScript|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|remediationScriptContent|Binary|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|runAs32Bit|Boolean|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|**TODO: Add Description**|
|deviceRunStates|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|**TODO: Add Description**|
|runSummary|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "detectionScriptContent": "Binary",
  "remediationScriptContent": "Binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": "Boolean",
  "highestAvailableVersion": "String"
}
```

