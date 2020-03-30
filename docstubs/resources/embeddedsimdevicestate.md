---
title: "embeddedSIMDeviceState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# embeddedSIMDeviceState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get embeddedSIMDeviceState](../api/embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Read properties and relationships of the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.|
|[Update embeddedSIMDeviceState](../api/embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Update the properties of a [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|deviceName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String||
|universalIntegratedCircuitCardIdentifier|String||
|userName|String||

## Relationships
None

## JSON representation
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

