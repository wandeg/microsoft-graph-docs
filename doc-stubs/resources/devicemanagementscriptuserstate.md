---
title: "deviceManagementScriptUserState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementScriptUserState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceRunStates](../api/devicemanagementscriptuserstate-list-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|Get the deviceManagementScriptDeviceStates from the deviceRunStates navigation property.|
|[Create deviceRunStates](../api/devicemanagementscriptuserstate-post-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Create a new deviceRunStates object.|
|[Delete deviceRunStates](../api/devicemanagementscriptuserstate-delete-devicerunstates.md)|None|Delete a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[Update deviceRunStates](../api/devicemanagementscriptuserstate-update-devicerunstates.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Update the properties of a deviceRunStates object.|
|[Get deviceManagementScriptDeviceState](../api/devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md)|Read the properties and relationships of a [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.|
|[List userRunStates](../api/devicemanagementscript-list-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md) collection|Get the deviceManagementScriptUserStates from the userRunStates navigation property.|
|[Create userRunStates](../api/devicemanagementscript-post-userrunstates.md)|[deviceManagementScriptUserState](../resources/devicemanagementscriptuserstate.md)|Create a new userRunStates object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|successDeviceCount|Int32|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "successDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "userPrincipalName": "String"
}
```

