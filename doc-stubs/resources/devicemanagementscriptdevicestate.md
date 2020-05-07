---
title: "deviceManagementScriptDeviceState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementScriptDeviceState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedDevice](../api/devicemanagementscriptdevicestate-list-manageddevice.md)|[managedDevice](../resources/manageddevice.md) collection|Get the managedDevices from the managedDevice navigation property.|
|[Add managedDevice](../api/devicemanagementscriptdevicestate-post-manageddevice.md)|[managedDevice](../resources/manageddevice.md)|Add managedDevice by posting to the managedDevice collection.|
|[Remove managedDevice](../api/devicemanagementscriptdevicestate-delete-manageddevice.md)|None|Remove a [managedDevice](../resources/manageddevice.md) object.|
|[List deviceRunStates](../api/devicemanagementscript-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Create deviceRunStates](../api/devicemanagementscript-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Create a new deviceRunStates object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorCode|Int32|**TODO: Add Description**|
|errorDescription|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastStateUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|resultMessage|String|**TODO: Add Description**|
|runState|runState|**TODO: Add Description**. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/manageddevice.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "errorCode": "Integer",
  "errorDescription": "String"
}
```

