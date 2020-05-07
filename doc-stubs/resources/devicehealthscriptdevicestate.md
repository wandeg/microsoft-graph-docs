---
title: "deviceHealthScriptDeviceState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptDeviceState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedDevice](../api/devicehealthscriptdevicestate-list-manageddevice.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevice navigation property.|
|[Add managedDevice](../api/devicehealthscriptdevicestate-post-manageddevice.md)|[managedDevice](../resources/manageddevice.md)|Add managedDevice by posting to the managedDevice collection.|
|[Remove managedDevice](../api/devicehealthscriptdevicestate-delete-manageddevice.md)|None|Remove a [managedDevice](../resources/manageddevice.md) object.|
|[List deviceRunStates](../api/devicehealthscript-list-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) collection|Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.|
|[Create deviceRunStates](../api/devicehealthscript-post-devicerunstates.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Create a new deviceRunStates object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionState|runState|**TODO: Add Description**. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|expectedStateUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastStateUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|postRemediationDetectionScriptError|String|**TODO: Add Description**|
|postRemediationDetectionScriptOutput|String|**TODO: Add Description**|
|preRemediationDetectionScriptError|String|**TODO: Add Description**|
|preRemediationDetectionScriptOutput|String|**TODO: Add Description**|
|remediationScriptError|String|**TODO: Add Description**|
|remediationState|remediationState|**TODO: Add Description**. Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/manageddevice.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "String (identifier)",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```

