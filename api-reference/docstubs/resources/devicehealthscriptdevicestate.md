---
title: "deviceHealthScriptDeviceState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScriptDeviceState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScriptDeviceState](../api/devicehealthscriptdevicestate-get.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.|
|[Update deviceHealthScriptDeviceState](../api/devicehealthscriptdevicestate-update.md)|[deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md)|Update the properties of a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read properties and relationships of the [managedDevice](../resources/manageddevice.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionState|Enumeration| Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|expectedStateUpdateDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastStateUpdateDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|postRemediationDetectionScriptError|String||
|postRemediationDetectionScriptOutput|String||
|preRemediationDetectionScriptError|String||
|preRemediationDetectionScriptOutput|String||
|remediationScriptError|String||
|remediationState|Enumeration| Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/manageddevice.md)||

## JSON representation
Here is a JSON representation of the resource.
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

