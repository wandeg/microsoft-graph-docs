---
title: "privilegedRoleAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# privilegedRoleAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoleAssignments](../api/privilegedroleassignment-list.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|List properties and relationships of the [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects.|
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Read properties and relationships of the [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[Create privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Create a new [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[Delete privilegedRoleAssignment](../api/privilegedroleassignment-delete.md)|None|Deletes a [privilegedRoleAssignment](../resources/privilegedroleassignment.md).|
|[Update privilegedRoleAssignment](../api/privilegedroleassignment-update.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Update the properties of a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)||
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)||
|[my](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection||
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedrole.md)|Read properties and relationships of the [privilegedRole](../resources/privilegedrole.md) object.|
|[List assignments](../api/privilegedrole-list-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|Get the privilegedRoleAssignments from the assignments navigation property.|
|[Create assignments](../api/privilegedrole-post-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Create assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isElevated|Boolean||
|resultMessage|String||
|roleId|String||
|userId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleInfo|[privilegedRole](../resources/privilegedrole.md)||

## JSON representation
Here is a JSON representation of the resource.
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
  "isElevated": true,
  "expirationDateTime": "String (timestamp)",
  "resultMessage": "String"
}
```

