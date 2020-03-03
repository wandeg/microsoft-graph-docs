---
title: "embeddedSIMDeviceState resource type"
description: "Describes the embedded SIM activation code deployment state in relation to a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# embeddedSIMDeviceState resource type


Namespace: microsoft.graph

Describes the embedded SIM activation code deployment state in relation to a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List embeddedSIMDeviceStates](../api/embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) collection|List properties and relationships of the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) objects.|
|[Get embeddedSIMDeviceState](../api/embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Read properties and relationships of the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.|
|[Create embeddedSIMDeviceState](../api/embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Create a new [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.|
|[Delete embeddedSIMDeviceState](../api/embeddedsimdevicestate-delete.md)|None|Deletes a [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md).|
|[Update embeddedSIMDeviceState](../api/embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Update the properties of a [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The time the embedded SIM device status was created. Generated service side.|
|deviceName|String|Device name to which the subscription was provisioned e.g. DESKTOP-JOE|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|The time the embedded SIM device last checked in. Updated service side.|
|modifiedDateTime|DateTimeOffset|The time the embedded SIM device status was last modified. Updated service side.|
|state|Enumeration|The state of the profile operation applied to the device. Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|String description of the provisioning state.|
|universalIntegratedCircuitCardIdentifier|String|The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.|
|userName|String|Username which the subscription was provisioned to e.g. joe@contoso.com|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```

