---
title: "deviceConfigurationGroupAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceConfigurationGroupAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceConfiguration](../api/deviceconfigurationgroupassignment-list-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md) collection|Get the deviceConfigurations from the deviceConfiguration navigation property.|
|[Add deviceConfiguration](../api/deviceconfigurationgroupassignment-post-deviceconfiguration.md)|[deviceConfiguration](../resources/deviceconfiguration.md)|Add deviceConfiguration by posting to the deviceConfiguration collection.|
|[Remove deviceConfiguration](../api/deviceconfigurationgroupassignment-delete-deviceconfiguration.md)|None|Remove a [deviceConfiguration](../resources/deviceconfiguration.md) object.|
|[List groupAssignments](../api/deviceconfiguration-list-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/deviceconfiguration-post-groupassignments.md)|[deviceConfigurationGroupAssignment](../resources/deviceconfigurationgroupassignment.md)|Create a new groupAssignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroup|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|targetGroupId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceConfiguration|[deviceConfiguration](../resources/deviceconfiguration.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "excludeGroup": "Boolean"
}
```

