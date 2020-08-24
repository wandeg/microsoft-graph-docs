---
title: "deviceHealthScript resource type"
description: "Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "resourcePageType"
---

# deviceHealthScript resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Intune will provide customer the ability to run their Powershell Health scripts (remediation + detection) on the enrolled windows 10 Azure Active Directory joined devices.

## Methods

| Method                                                                                                               | Return Type                                                   | Description                                                                       |
| :------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------ | :-------------------------------------------------------------------------------- |
| [List deviceHealthScript](../api/intune-devicehealthscript-list.md)                                                  | [deviceHealthScript](intune-deviceHealthScript.md) collection | List properties and relationships of a deviceHealthScript object.                 |
| [Create deviceHealthScript](../api/intune-devicehealthscript-create.md)                                              | [deviceHealthScript](intune-deviceHealthScript.md)            | Create a new deviceHealthScript object.                                           |
| [Get deviceHealthScript](../api/intune-devicehealthscript-get.md)                                                    | [deviceHealthScript](intune-deviceHealthScript.md)            | Read properties and relationships of a deviceHealthScript object.                 |
| [Update deviceHealthScript](../api/intune-devicehealthscript-update.md)                                              | [deviceHealthScript](intune-deviceHealthScript.md)            | Update the properties of a deviceHealthScript object.                             |
| [Delete deviceHealthScript](../api/intune-devicehealthscript-delete.md)                                              |                                                               | Delete a deviceHealthScript object.                                               |
| [assign](../api/intune-devicehealthscript-assign.md)                                                                 |                                                               |                                                                                   |
| [enableGlobalScripts](../api/intune-devicehealthscript-enableGlobalScripts.md)                                       |                                                               |                                                                                   |
| [getGlobalScriptHighestAvailableVersion](../api/intune-devicehealthscript-getGlobalScriptHighestAvailableVersion.md) | String                                                        | Update the Proprietary Device Health Script                                       |
| [updateGlobalScript](../api/intune-devicehealthscript-updateGlobalScript.md)                                         | String                                                        | Update the Proprietary Device Health Script                                       |
| [areGlobalScriptsAvailable](../api/intune-devicehealthscript-areGlobalScriptsAvailable.md)                           | globalDeviceHealthScriptState                                 |                                                                                   |
| [getRemediationHistory](../api/intune-devicehealthscript-getRemediationHistory.md)                                   | deviceHealthScriptRemediationHistory                          | Function to get the number of remediations by a device health scripts             |
| [getRemediationSummary](../api/intune-devicehealthscript-getRemediationSummary.md)                                   | deviceHealthScriptRemediationSummary                          |                                                                                   |
| [List assignments](../api/intune-devicehealthscript-list-assignments.md)                                             | deviceHealthScriptAssignment                                  | Get the deviceHealthScriptAssignment from an assignments navigation property.     |
| [Create assignments](../api/intune-devicehealthscript-post-assignments.md)                                           | deviceHealthScriptAssignment                                  | Create a new assignments object.                                                  |
| [Get assignments](../api/intune-devicehealthscript-get-assignments.md)                                               | deviceHealthScriptAssignment                                  | Read the properties and relationships of a deviceHealthScriptAssignment object.   |
| [Update assignments](../api/intune-devicehealthscript-update-assignments.md)                                         | deviceHealthScriptAssignment                                  | Update the properties of an assignments object.                                   |
| [Delete assignments](../api/intune-devicehealthscript-delete-assignments.md)                                         |                                                               | Delete a deviceHealthScriptAssignment object.                                     |
| [List deviceRunStates](../api/intune-devicehealthscript-list-devicerunstates.md)                                     | deviceHealthScriptDeviceState                                 | Get the deviceHealthScriptDeviceState from a deviceRunStates navigation property. |
| [Create deviceRunStates](../api/intune-devicehealthscript-post-devicerunstates.md)                                   | deviceHealthScriptDeviceState                                 | Create a new deviceRunStates object.                                              |
| [Get deviceRunStates](../api/intune-devicehealthscript-get-devicerunstates.md)                                       | deviceHealthScriptDeviceState                                 | Read the properties and relationships of a deviceHealthScriptDeviceState object.  |
| [Update deviceRunStates](../api/intune-devicehealthscript-update-devicerunstates.md)                                 | deviceHealthScriptDeviceState                                 | Update the properties of a deviceRunStates object.                                |
| [Delete deviceRunStates](../api/intune-devicehealthscript-delete-devicerunstates.md)                                 |                                                               | Delete a deviceHealthScriptDeviceState object.                                    |
| [List runSummary](../api/intune-devicehealthscript-list-runsummary.md)                                               | deviceHealthScriptRunSummary                                  | Get the deviceHealthScriptRunSummary from a runSummary navigation property.       |
| [Create runSummary](../api/intune-devicehealthscript-post-runsummary.md)                                             | deviceHealthScriptRunSummary                                  | Create a new runSummary object.                                                   |
| [Get runSummary](../api/intune-devicehealthscript-get-runsummary.md)                                                 | deviceHealthScriptRunSummary                                  | Read the properties and relationships of a deviceHealthScriptRunSummary object.   |
| [Update runSummary](../api/intune-devicehealthscript-update-runsummary.md)                                           | deviceHealthScriptRunSummary                                  | Update the properties of a runSummary object.                                     |
| [Delete runSummary](../api/intune-devicehealthscript-delete-runsummary.md)                                           |                                                               | Delete a deviceHealthScriptRunSummary object.                                     |

## Properties

| Property                    | Type                                                                                  | Description                                                                              |
| :-------------------------- | :------------------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------- |
| createdDateTime             | DateTimeOffset                                                                        | The timestamp of when the device health script was created. This property is read-only.  |
| description                 | String                                                                                | Description of the device health script                                                  |
| detectionScriptContent      | Binary                                                                                | The entire content of the detection powershell script                                    |
| detectionScriptParameters   | [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md) collection | List of ComplexType DetectionScriptParameters objects.                                   |
| displayName                 | String                                                                                | Name of the device health script                                                         |
| enforceSignatureCheck       | Boolean                                                                               | Indicate whether the script signature needs be checked                                   |
| highestAvailableVersion     | String                                                                                | Highest available version for a Microsoft Proprietary script                             |
| id                          | String                                                                                | Unique Identifier for the device health script Read-only.                                |
| isGlobalScript              | Boolean                                                                               | Determines if this is Microsoft Proprietary Script. Proprietary scripts are read-only    |
| lastModifiedDateTime        | DateTimeOffset                                                                        | The timestamp of when the device health script was modified. This property is read-only. |
| publisher                   | String                                                                                | Name of the device health script publisher                                               |
| remediationScriptContent    | Binary                                                                                | The entire content of the remediation powershell script                                  |
| remediationScriptParameters | [deviceHealthScriptParameter](../resources/devicehealthscriptparameter.md) collection | List of ComplexType RemediationScriptParameters objects.                                 |
| roleScopeTagIds             | String collection                                                                     | List of Scope Tag IDs for the device health script                                       |
| runAs32Bit                  | Boolean                                                                               | Indicate whether PowerShell script(s) should run as 32-bit                               |
| runAsAccount                | String                                                                                | Indicates the type of execution context                                                  |
| version                     | String                                                                                | Version of the device health script                                                      |

## Relationships

| Relationship    | Type                                                                                      | Description                                                        |
| :-------------- | :---------------------------------------------------------------------------------------- | :----------------------------------------------------------------- |
| assignments     | [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection   | The list of group assignments for the device health script         |
| deviceRunStates | [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection | List of run states for the device health script across all devices |
| runSummary      | [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md)              | High level run summary for device health script.                   |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript",
  "baseType": "microsoft.graph.entity",
  "openType": False
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "createdDateTime": "DateTimeOffset",
  "description": "String",
  "detectionScriptContent": "Binary",
  "detectionScriptParameters": [{"@odata.type": "microsoft.graph.deviceHealthScriptParameter"}],
  "displayName": "String",
  "enforceSignatureCheck": "Boolean",
  "highestAvailableVersion": "String",
  "id": "String (identifier)",
  "isGlobalScript": "Boolean",
  "lastModifiedDateTime": "DateTimeOffset",
  "publisher": "String",
  "remediationScriptContent": "Binary",
  "remediationScriptParameters": [{"@odata.type": "microsoft.graph.deviceHealthScriptParameter"}],
  "roleScopeTagIds": ["String"],
  "runAs32Bit": "Boolean",
  "runAsAccount": "system | user",
  "version": "String"
}
```