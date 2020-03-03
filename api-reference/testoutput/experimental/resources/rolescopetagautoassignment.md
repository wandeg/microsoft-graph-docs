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
|[List roleScopeTagAutoAssignments](../api/rolescopetagautoassignment-list.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|List properties and relationships of the [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) objects.|
|[Get roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Create roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Create a new [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Delete roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-delete.md)|None|Deletes a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md).|
|[Update roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Update the properties of a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The auto-assignment target for the specific Role Scope Tag.|

## Relationships
None

## JSON Representation
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

