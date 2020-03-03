---
title: "roleScopeTag resource type"
description: "Role Scope Tag"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleScopeTag resource type


Namespace: microsoft.graph

Role Scope Tag


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List roleScopeTags](../api/rolescopetag-list.md)|[roleScopeTag](../resources/rolescopetag.md) collection|List properties and relationships of the [roleScopeTag](../resources/rolescopetag.md) objects.|
|[Get roleScopeTag](../api/rolescopetag-get.md)|[roleScopeTag](../resources/rolescopetag.md)|Read properties and relationships of the [roleScopeTag](../resources/rolescopetag.md) object.|
|[Create roleScopeTag](../api/rolescopetag-create.md)|[roleScopeTag](../resources/rolescopetag.md)|Create a new [roleScopeTag](../resources/rolescopetag.md) object.|
|[Delete roleScopeTag](../api/rolescopetag-delete.md)|None|Deletes a [roleScopeTag](../resources/rolescopetag.md).|
|[Update roleScopeTag](../api/rolescopetag-update.md)|[roleScopeTag](../resources/rolescopetag.md)|Update the properties of a [roleScopeTag](../resources/rolescopetag.md) object.|
|[assign](../api/rolescopetag-assign.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection||
|[getRoleScopeTagsById](../api/rolescopetag-getrolescopetagsbyid.md)|[roleScopeTag](../resources/rolescopetag.md) collection||
|[hasCustomRoleScopeTag](../api/rolescopetag-hascustomrolescopetag.md)|Boolean||
|[List assignments](../api/rolescopetag-list-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|Get the roleScopeTagAutoAssignments from the assignments navigation property.|
|[Add assignments](../api/rolescopetag-post-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role Scope Tag.|
|displayName|String|The display or friendly name of the Role Scope Tag.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|Description of the Role Scope Tag.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|The list of assignments for this Role Scope Tag.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isBuiltIn": true
}
```

