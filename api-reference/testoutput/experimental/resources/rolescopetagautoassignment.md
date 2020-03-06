---
title: "roleScopeTagAutoAssignment resource type"
description: "Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleScopeTagAutoAssignment resource type


Namespace: microsoft.graph

Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Update roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Update the properties of a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[List assignments](../api/rolescopetag-list-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|Get the roleScopeTagAutoAssignments from the assignments navigation property.|
|[Add assignments](../api/rolescopetag-post-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The auto-assignment target for the specific Role Scope Tag.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

