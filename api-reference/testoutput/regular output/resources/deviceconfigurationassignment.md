---
title: "deviceConfigurationAssignment resource type"
description: "The device configuration assignment entity assigns an AAD group to a specific device configuration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationAssignment resource type


Namespace: microsoft.graph

The device configuration assignment entity assigns an AAD group to a specific device configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceConfigurationAssignments](../api/deviceconfigurationassignment-list.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) collection|List properties and relationships of the [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) objects.|
|[Get deviceConfigurationAssignment](../api/deviceconfigurationassignment-get.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Read properties and relationships of the [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[Create deviceConfigurationAssignment](../api/deviceconfigurationassignment-create.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Create a new [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|
|[Delete deviceConfigurationAssignment](../api/deviceconfigurationassignment-delete.md)|None|Deletes a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md).|
|[Update deviceConfigurationAssignment](../api/deviceconfigurationassignment-update.md)|[deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md)|Update the properties of a [deviceConfigurationAssignment](../resources/deviceconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The assignment target for the device configuration.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

