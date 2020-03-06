---
title: "deviceManagementScriptUserState resource type"
description: "Contains properties for user run state of the device management script."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScriptUserState resource type


Namespace: microsoft.graph

Contains properties for user run state of the device management script.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementScriptUserState](../api/devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Read properties and relationships of the [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.|
|[Update deviceManagementScriptUserState](../api/devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Update the properties of a [deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) object.|
|[List deviceRunStates](../api/devicemanagementscriptuserstate-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Add deviceRunStates](../api/devicemanagementscriptuserstate-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Add deviceRunStates by posting to the deviceRunStates collection.|
|[List userRunStates](../api/devicemanagementscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Add userRunStates](../api/devicemanagementscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Add userRunStates by posting to the userRunStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDeviceCount|Int32|Error device count for specific user.|
|id|String| Inherited from [entity](../resources/entity.md)|
|successDeviceCount|Int32|Success device count for specific user.|
|userPrincipalName|String|User principle name of specific user.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|List of run states for this script across all devices of specific user.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```

