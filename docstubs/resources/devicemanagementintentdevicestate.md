---
title: "deviceManagementIntentDeviceState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntentDeviceState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentDeviceState](../api/devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|
|[Update deviceManagementIntentDeviceState](../api/devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Update the properties of a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|
|[List deviceStates](../api/devicemanagementintent-list-devicestates.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) collection|Get the deviceManagementIntentDeviceStates from the deviceStates navigation property.|
|[Add deviceStates](../api/devicemanagementintent-post-devicestates.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Add deviceStates by posting to the deviceStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String||
|deviceId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userName|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```

