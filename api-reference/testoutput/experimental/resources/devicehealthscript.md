---
title: "deviceHealthScript resource type"
description: "Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScript resource type


Namespace: microsoft.graph

Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScript](../api/devicehealthscript-get.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Read properties and relationships of the [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[Update deviceHealthScript](../api/devicehealthscript-update.md)|[deviceHealthScript](../resources/devicehealthscript.md)|Update the properties of a [deviceHealthScript](../resources/devicehealthscript.md) object.|
|[assign](../api/devicehealthscript-assign.md)|None||
|[List assignments](../api/devicehealthscript-list-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|Get the deviceHealthScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/devicehealthscript-post-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Add assignments by posting to the assignments collection.|
|[Get deviceHealthScriptRunSummary](../api/devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)|Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.|
|[List deviceRunStates](../api/devicehealthscript-list-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/devicehealthscript-post-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|

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
  ]
}
```

