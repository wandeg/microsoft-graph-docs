---
title: "embeddedSIMActivationCodePoolAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# embeddedSIMActivationCodePoolAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get embeddedSIMActivationCodePoolAssignment](../api/embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) object.|
|[Update embeddedSIMActivationCodePoolAssignment](../api/embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) object.|
|[List assignments](../api/embeddedsimactivationcodepool-list-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md) collection|Get the embeddedSIMActivationCodePoolAssignments from the assignments navigation property.|
|[Add assignments](../api/embeddedsimactivationcodepool-post-assignments.md)|[embeddedSIMActivationCodePoolAssignment](../resources/embeddedsimactivationcodepoolassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

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

