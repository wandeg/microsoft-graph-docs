---
title: "deviceManagementIntentAssignment resource type"
description: "Intent assignment entity"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntentAssignment resource type


Namespace: microsoft.graph

Intent assignment entity


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentAssignment](../api/devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Read properties and relationships of the [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Update deviceManagementIntentAssignment](../api/devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Update the properties of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[List assignments](../api/devicemanagementintent-list-assignments.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) collection|Get the deviceManagementIntentAssignments from the assignments navigation property.|
|[Add assignments](../api/devicemanagementintent-post-assignments.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The assignment target|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

