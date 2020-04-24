---
title: "deviceManagementIntentAssignment resource type"
description: "Intent assignment entity"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntentAssignment resource type


Namespace: microsoft.graph

Intent assignment entity


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentAssignment](../api/devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Read the properties and relationships of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|
|[Update deviceManagementIntentAssignment](../api/devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md)|Update the properties of a [deviceManagementIntentAssignment](../resources/devicemanagementintentassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

