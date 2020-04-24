---
title: "embeddedSIMActivationCodePoolAssignment resource type"
description: "The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# embeddedSIMActivationCodePoolAssignment resource type


Namespace: microsoft.graph

The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get embeddedSIMActivationCodePoolAssignment](../api/embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Read the properties and relationships of an [embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) object.|
|[Update embeddedSIMActivationCodePoolAssignment](../api/embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Update the properties of an [embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The type of groups targeted by the embedded SIM activation code pool.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

