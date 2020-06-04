---
title: "privilegedRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedRoleAssignment resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List assignments](../api/privilegedrole-list-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|Get the privilegedRoleAssignments from the assignments navigation property.|
|[Add assignments](../api/privilegedrole-post-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Add assignments by posting to the assignments collection.|
|[Remove assignments](../api/privilegedrole-delete-assignments.md)|None|Remove a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[List privilegedRoleAssignments](../api/privilegedroleassignment-list.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|Get a list of the [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects and their properties.|
|[Create privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Create a new [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Read the properties and relationships of a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[Update privilegedRoleAssignment](../api/privilegedroleassignment-update.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Update the properties of a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[Delete privilegedRoleAssignment](../api/privilegedroleassignment-delete.md)|None|Deletes a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|**TODO: Add Description**|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|**TODO: Add Description**|
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|**TODO: Add Description**|
|[List roleInfo](../api/privilegedroleassignment-list-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md) collection|Get the privilegedRoles from the roleInfo navigation property.|
|[Create roleInfo](../api/privilegedroleassignment-post-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Create a new roleInfo object.|
|[Get roleInfo](../api/privilegedroleassignment-get-privilegedrole.md)|[privilegedRole](../resources/privilegedrole.md)|Read the properties and relationships of a [privilegedRole](../resources/privilegedrole.md) object.|
|[Update roleInfo](../api/privilegedroleassignment-update-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Update the properties of a roleInfo object.|
|[Delete roleInfo](../api/privilegedroleassignment-delete-roleinfo.md)|None|Delete a [privilegedRole](../resources/privilegedrole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isElevated|Boolean|**TODO: Add Description**|
|resultMessage|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleInfo|[privilegedRole](../resources/privilegedrole.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "id": "String (identifier)",
  "userId": "String",
  "roleId": "String",
  "isElevated": "Boolean",
  "expirationDateTime": "String (timestamp)",
  "resultMessage": "String"
}
```

