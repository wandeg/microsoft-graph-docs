---
title: "embeddedSIMActivationCodePool resource type"
description: "A pool represents a group of embedded SIM activation codes."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# embeddedSIMActivationCodePool resource type


Namespace: microsoft.graph

A pool represents a group of embedded SIM activation codes.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[Update embeddedSIMActivationCodePool](../api/embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md)|Update the properties of a [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) object.|
|[assign](../api/embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) collection||
|[List assignments](../api/embeddedsimactivationcodepool-list-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) collection|Get the embeddedSIMActivationCodePoolAssignments from the assignments navigation property.|
|[Add assignments](../api/embeddedsimactivationcodepool-post-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStates](../api/embeddedsimactivationcodepool-list-devicestates.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) collection|Get the embeddedSIMDeviceStates from the deviceStates navigation property.|
|[Add deviceStates](../api/embeddedsimactivationcodepool-post-devicestates.md)|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md)|Add deviceStates by posting to the deviceStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activationCodeCount|Int32|The total count of activation codes which belong to this pool.|
|activationCodes|[embeddedSIMActivationCode](../resources/embeddedsimactivationcode.md) collection|The activation codes which belong to this pool. This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.|
|createdDateTime|DateTimeOffset|The time the embedded SIM activation code pool was created. Generated service side.|
|displayName|String|The admin defined name of the embedded SIM activation code pool.|
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|The time the embedded SIM activation code pool was last modified. Updated service side.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) collection|Navigational property to a list of targets to which this pool is assigned.|
|deviceStates|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) collection|Navigational property to a list of device states for this pool.|

## JSON representation
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

