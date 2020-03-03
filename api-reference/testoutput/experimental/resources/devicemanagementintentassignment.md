---
title: "deviceManagementIntentAssignment resource type"
description: "Intent assignment entity"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementIntentAssignment resource type

Intent assignment entity


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentAssignment](../api/devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/deviceManagementIntentAssignment.md)|Read properties and relationships of the [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Delete deviceManagementIntentAssignment](../api/devicemanagementintentassignment-delete.md)|None|Deletes a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md).|
|[Update deviceManagementIntentAssignment](../api/devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/deviceManagementIntentAssignment.md)|Update the properties of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceAndAppManagementAssignmentTarget.md)|The assignment target|

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

