---
title: "roleScopeTag resource type"
description: "Role Scope Tag"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleScopeTag resource type


Namespace: microsoft.graph

Role Scope Tag


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleScopeTag](../api/rolescopetag-get.md)|[roleScopeTag](../resources/rolescopetag.md)|Read the properties and relationships of a [roleScopeTag](../resources/rolescopetag.md) object.|
|[Update roleScopeTag](../api/rolescopetag-update.md)|[roleScopeTag](../resources/rolescopetag.md)|Update the properties of a [roleScopeTag](../resources/rolescopetag.md) object.|
|[assign](../api/rolescopetag-assign.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|**TODO: Add Description**|
|[getRoleScopeTagsById](../api/rolescopetag-getrolescopetagsbyid.md)|[roleScopeTag](../resources/rolescopetag.md) collection|**TODO: Add Description**|
|[hasCustomRoleScopeTag](../api/rolescopetag-hascustomrolescopetag.md)|Boolean|**TODO: Add Description**|
|[List assignments](../api/rolescopetag-list-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|Get the roleScopeTagAutoAssignments from the assignments navigation property.|
|[Create assignments](../api/rolescopetag-post-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/rolescopetag-delete-assignments.md)|None|Delete an [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Update assignments](../api/rolescopetag-update-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Update the properties of an assignments object.|
|[Get roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Read the properties and relationships of a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role Scope Tag.|
|displayName|String|The display or friendly name of the Role Scope Tag.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|Description of the Role Scope Tag.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|The list of assignments for this Role Scope Tag.|

## JSON representation
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

