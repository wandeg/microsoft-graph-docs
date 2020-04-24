---
title: "deviceConfigurationGroupAssignment resource type"
description: "Device configuration group assignment."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceConfigurationGroupAssignment resource type


Namespace: microsoft.graph

Device configuration group assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceConfigurationGroupAssignment](../api/deviceconfigurationgroupassignment-get.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Read the properties and relationships of a [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[Update deviceConfigurationGroupAssignment](../api/deviceconfigurationgroupassignment-update.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Update the properties of a [deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) object.|
|[List deviceConfiguration](../api/deviceconfigurationgroupassignment-list-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md) collection|Get the deviceConfigurations from the deviceConfiguration navigation property.|
|[Add deviceConfiguration](../api/deviceconfigurationgroupassignment-post-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Add deviceConfiguration by posting to the deviceConfiguration collection.|
|[Remove deviceConfiguration](../api/deviceconfigurationgroupassignment-delete-deviceconfiguration.md)|None|Remove a [deviceConfiguration](../resources/deviceconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroup|Boolean|Indicates if this group is should be excluded. Defaults that the group should be included|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

