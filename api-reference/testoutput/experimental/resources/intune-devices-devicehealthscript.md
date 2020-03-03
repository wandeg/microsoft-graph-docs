---
title: "deviceHealthScript resource type"
description: "Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceHealthScript resource type

Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md)|Read properties and relationships of the [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[Delete deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|None|Deletes a [deviceHealthScript](../resources/devicehealthscript.md).|
|[Update deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md)|Update the properties of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[assign](../api/intune-devices-devicehealthscript-assign.md)|None||
|[List assignments](../api/intune-devices-devicehealthscript-list-assignments.md)|[deviceHealthScriptAssignment](../resources/intune-devices-deviceHealthScriptAssignment.md) collection|Get the deviceHealthScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/intune-devices-devicehealthscript-post-assignments.md)|[deviceHealthScriptAssignment](../resources/intune-devices-deviceHealthScriptAssignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-deviceHealthScriptRunSummary.md)|Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[List deviceRunStates](../api/intune-devices-devicehealthscript-list-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-deviceHealthScriptDeviceState.md) collection|Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/intune-devices-devicehealthscript-post-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/intune-devices-deviceHealthScriptDeviceState.md)|Add deviceRunStates by posting to the deviceRunStates collection.|
|[List deviceHealthScripts](../api/intune-devices-devicemanagement-list-devicehealthscripts.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md) collection|Get the deviceHealthScripts from the deviceHealthScripts navigation property.|
|[Add deviceHealthScripts](../api/intune-devices-devicemanagement-post-devicehealthscripts.md)|[deviceHealthScript](../resources/intune-devices-deviceHealthScript.md)|Add deviceHealthScripts by posting to the deviceHealthScripts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The timestamp of when the device health script was created. This property is read-only.|
|description|String|Description of the device health script|
|detectionScriptContent|Binary|The entire content of the detection powershell script|
|displayName|String|Name of the device health script|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The timestamp of when the device health script was modified. This property is read-only.|
|publisher|String|Name of the device health script publisher|
|remediationScriptContent|Binary|The entire content of the remediation powershell script|
|roleScopeTagIds|String collection|List of Scope Tag IDs for the device health script|
|runAs32Bit|Boolean|Indicate whether PowerShell script(s) should run as 32-bit|
|runAsAccount|Enumeration|Indicates the type of execution context. Possible values are: `system`, `user`.|
|version|String|Version of the device health script|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[deviceHealthScriptAssignment](../resources/intune-devices-deviceHealthScriptAssignment.md) collection|The list of group assignments for the device health script|
|deviceRunStates|[deviceHealthScriptDeviceState](../resources/intune-devices-deviceHealthScriptDeviceState.md) collection|List of run states for the device health script across all devices|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-deviceHealthScriptRunSummary.md)|High level run summary for device health script.|

## JSON Representation
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
  ]
}
```

