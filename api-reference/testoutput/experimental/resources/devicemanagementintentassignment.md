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
|[List deviceManagementIntentAssignments](../api/devicemanagementintentassignment-list.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) collection|List properties and relationships of the [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) objects.|
|[Get deviceManagementIntentAssignment](../api/devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Read properties and relationships of the [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Create deviceManagementIntentAssignment](../api/devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Create a new [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Delete deviceManagementIntentAssignment](../api/devicemanagementintentassignment-delete.md)|None|Deletes a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md).|
|[Update deviceManagementIntentAssignment](../api/devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Update the properties of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The assignment target|

## Relationships
None

## JSON Representation
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

