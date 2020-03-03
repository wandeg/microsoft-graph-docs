---
title: "embeddedSIMActivationCodePool resource type"
description: "A pool represents a group of embedded SIM activation codes."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# embeddedSIMActivationCodePool resource type

A pool represents a group of embedded SIM activation codes.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md)|Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[Delete embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-delete.md)|None|Deletes a [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md).|
|[Update embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md)|Update the properties of a [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[assign](../api/embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedSIMActivationCodePoolAssignment.md) collection||
|[List assignments](../api/embeddedsimactivationcodepool-list-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedSIMActivationCodePoolAssignment.md) collection|Get the embeddedSIMActivationCodePoolAssignments from the assignments navigation property.|
|[Add assignments](../api/embeddedsimactivationcodepool-post-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedSIMActivationCodePoolAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStates](../api/embeddedsimactivationcodepool-list-devicestates.md)|[embeddedSIMDeviceState](../resources/embeddedSIMDeviceState.md) collection|Get the embeddedSIMDeviceStates from the deviceStates navigation property.|
|[Add deviceStates](../api/embeddedsimactivationcodepool-post-devicestates.md)|[embeddedSIMDeviceState](../resources/embeddedSIMDeviceState.md)|Add deviceStates by posting to the deviceStates collection.|
|[List embeddedSIMActivationCodePools](../api/intune-devices-devicemanagement-list-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md) collection|Get the embeddedSIMActivationCodePools from the embeddedSIMActivationCodePools navigation property.|
|[Add embeddedSIMActivationCodePools](../api/intune-devices-devicemanagement-post-embeddedsimactivationcodepools.md)|[embeddedSIMActivationCodePool](../resources/embeddedSIMActivationCodePool.md)|Add embeddedSIMActivationCodePools by posting to the embeddedSIMActivationCodePools collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activationCodeCount|Int32|The total count of activation codes which belong to this pool.|
|activationCodes|[embeddedSIMActivationCode](../resources/embeddedSIMActivationCode.md) collection|The activation codes which belong to this pool. This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.|
|createdDateTime|DateTimeOffset|The time the embedded SIM activation code pool was created. Generated service side.|
|displayName|String|The admin defined name of the embedded SIM activation code pool.|
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|The time the embedded SIM activation code pool was last modified. Updated service side.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedSIMActivationCodePoolAssignment.md) collection|Navigational property to a list of targets to which this pool is assigned.|
|deviceStates|[embeddedSIMDeviceState](../resources/embeddedSIMDeviceState.md) collection|Navigational property to a list of device states for this pool.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```

