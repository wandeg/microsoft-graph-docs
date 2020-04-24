---
title: "deviceHealthScript resource type"
description: "Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScript resource type


Namespace: microsoft.graph

Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScript](../api/devicehealthscript-get.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Read the properties and relationships of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[Update deviceHealthScript](../api/devicehealthscript-update.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Update the properties of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
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
|createdDateTime|DateTimeOffset|The timestamp of when the device health script was created. This property is read-only.|
|description|String|Description of the device health script|
|detectionScriptContent|Binary|The entire content of the detection powershell script|
|displayName|String|Name of the device health script|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked|
|highestAvailableVersion|String|Highest available version for a Microsoft Proprietary script|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isGlobalScript|Boolean|Determines if this is Microsoft Proprietary Script. Proprietary scripts are read-only|
|lastModifiedDateTime|DateTimeOffset|The timestamp of when the device health script was modified. This property is read-only.|
|publisher|String|Name of the device health script publisher|
|remediationScriptContent|Binary|The entire content of the remediation powershell script|
|roleScopeTagIds|String collection|List of Scope Tag IDs for the device health script|
|runAs32Bit|Boolean|Indicate whether PowerShell script(s) should run as 32-bit|
|runAsAccount|runAsAccountType|Indicates the type of execution context. Possible values are: `system`, `user`.|
|version|String|Version of the device health script|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|The list of group assignments for the device health script|
|deviceRunStates|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|List of run states for the device health script across all devices|
|runSummary|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|High level run summary for device health script.|

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

