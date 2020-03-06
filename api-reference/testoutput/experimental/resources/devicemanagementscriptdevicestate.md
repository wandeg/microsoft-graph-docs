---
title: "deviceManagementScriptDeviceState resource type"
description: "Contains properties for device run state of the device management script."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScriptDeviceState resource type


Namespace: microsoft.graph

Contains properties for device run state of the device management script.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementScriptDeviceState](../api/devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[Update deviceManagementScriptDeviceState](../api/devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Update the properties of a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[Get managedDevice](../api/manageddevice-get.md)|[managedDevice](../resources/manageddevice.md)|Read properties and relationships of the [managedDevice](../resources/manageddevice.md) object.|
|[List deviceRunStates](../api/devicemanagementscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/devicemanagementscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorCode|Int32|Error code corresponding to erroneous execution of the device management script.|
|errorDescription|String|Error description corresponding to erroneous execution of the device management script.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastStateUpdateDateTime|DateTimeOffset|Latest time the device management script executes.|
|resultMessage|String|Details of execution output.|
|runState|Enumeration|State of latest run of the device management script. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/manageddevice.md)|The managed devices that executes the device management script.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```

