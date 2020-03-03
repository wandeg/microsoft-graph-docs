---
title: "privilegedRole resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedRole resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoles](../api/privilegedrole-list.md)|[privilegedRole](../resources/privilegedRole.md) collection|List properties and relationships of the [privilegedRole](../resources/privilegedrole.md) objects.|
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedRole.md)|Read properties and relationships of the [privilegedRole](../resources/privilegedrole.md) object.|
|[Create privilegedRole](../api/privilegedrole-post-privilegedroles.md)|[privilegedRole](../resources/privilegedRole.md)|Create a new [privilegedRole](../resources/privilegedrole.md) object.|
|[Delete privilegedRole](../api/privilegedrole-delete.md)|None|Deletes a [privilegedRole](../resources/privilegedrole.md).|
|[Update privilegedRole](../api/privilegedrole-update.md)|[privilegedRole](../resources/privilegedRole.md)|Update the properties of a [privilegedRole](../resources/privilegedrole.md) object.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](../resources/privilegedRoleAssignment.md)||
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](../resources/privilegedRoleAssignment.md)||
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)|Read properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[List assignments](../api/privilegedrole-list-assignments.md)|[privilegedRoleAssignment](../resources/privilegedRoleAssignment.md) collection|Get the privilegedRoleAssignments from the assignments navigation property.|
|[Create assignments](../api/privilegedrole-post-assignments.md)|[privilegedRoleAssignment](../resources/privilegedRoleAssignment.md)|Create assignments by posting to the assignments collection.|
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md)|[privilegedRoleSummary](../resources/privilegedRoleSummary.md)|Read properties and relationships of the [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[privilegedRoleAssignment](../resources/privilegedRoleAssignment.md) collection||
|settings|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)||
|summary|[privilegedRoleSummary](../resources/privilegedRoleSummary.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRole",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedRole",
  "id": "String (identifier)",
  "name": "String"
}
```

