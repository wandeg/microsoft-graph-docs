---
title: "roleScopeTag resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleScopeTag resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/rolescopetag-assign.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|**TODO: Add Description**|
|[getRoleScopeTagsById](../api/rolescopetag-getrolescopetagsbyid.md)|[roleScopeTag](../resources/rolescopetag.md) collection|**TODO: Add Description**|
|[hasCustomRoleScopeTag](../api/rolescopetag-hascustomrolescopetag.md)|Boolean|**TODO: Add Description**|
|[List assignments](../api/rolescopetag-list-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|Get the roleScopeTagAutoAssignments from the assignments navigation property.|
|[Create assignments](../api/rolescopetag-post-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/rolescopetag-delete-assignments.md)|None|Delete an [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Update assignments](../api/rolescopetag-update-assignments.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Update the properties of an assignments object.|
|[Get roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Read the properties and relationships of a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[List roleScopeTags](../api/deviceandappmanagementroleassignment-list-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md) collection|Get the roleScopeTags from the roleScopeTags navigation property.|
|[Add roleScopeTags](../api/deviceandappmanagementroleassignment-post-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md)|Add roleScopeTags by posting to the roleScopeTags collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "isBuiltIn": "Boolean"
}
```

