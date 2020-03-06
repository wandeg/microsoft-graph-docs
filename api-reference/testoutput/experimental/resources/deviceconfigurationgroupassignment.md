---
title: "deviceConfigurationGroupAssignment resource type"
description: "Device configuration group assignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceConfigurationGroupAssignment resource type


Namespace: microsoft.graph

Device configuration group assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationGroupAssignment](../api/deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[Update deviceConfigurationGroupAssignment](../api/deviceconfigurationgroupassignment-update.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Update the properties of a [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[Get deviceConfiguration](../api/deviceconfiguration-get.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Read properties and relationships of the [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[List groupAssignments](../api/deviceconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/deviceconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroup|Boolean|Indicates if this group is should be excluded. Defaults that the group should be included|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|The Id of the AAD group we are targeting the device configuration to.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceConfiguration|[deviceConfiguration](../resources/deviceconfiguration.md)|The navigation link to the Device Configuration being targeted.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```

