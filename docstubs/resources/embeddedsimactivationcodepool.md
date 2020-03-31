---
title: "embeddedSIMActivationCodePool resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# embeddedSIMActivationCodePool resource type


Namespace: microsoft.graph




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
|activationCodeCount|Int32||
|activationCodes|[embeddedSIMActivationCode](../resources/embeddedsimactivationcode.md) collection||
|createdDateTime|DateTimeOffset||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) collection||
|deviceStates|[embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) collection||

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

