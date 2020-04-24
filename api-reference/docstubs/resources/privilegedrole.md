---
title: "privilegedRole resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedRole resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoles](../api/privilegedrole-list.md)|[privilegedRole](../resources/privilegedrole.md) collection|Get a list of the [privilegedRole](../resources/privilegedrole.md) objects and their properties.|
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedrole.md)|Read the properties and relationships of a [privilegedRole](../resources/privilegedrole.md) object.|
|[Create privilegedRole](../api/privilegedrole-post-privilegedroles.md)|[privilegedRole](../resources/privilegedrole.md)|Create a new [privilegedRole](../resources/privilegedrole.md) object.|
|[Delete privilegedRole](../api/privilegedrole-delete.md)|None|Deletes a [privilegedRole](../resources/privilegedrole.md) object.|
|[Update privilegedRole](../api/privilegedrole-update.md)|[privilegedRole](../resources/privilegedrole.md)|Update the properties of a [privilegedRole](../resources/privilegedrole.md) object.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|**TODO: Add Description**|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|**TODO: Add Description**|
|[List settings](../api/privilegedrole-list-settings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md) collection|Get the privilegedRoleSettings from the settings navigation property.|
|[Create settings](../api/privilegedrole-post-settings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Create a new settings object.|
|[Delete settings](../api/privilegedrole-delete-settings.md)|None|Delete a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Update settings](../api/privilegedrole-update-settings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Update the properties of a settings object.|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Read the properties and relationships of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[List assignments](../api/privilegedrole-list-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|Get the privilegedRoleAssignments from the assignments navigation property.|
|[Add assignments](../api/privilegedrole-post-assignments.md)|[privilegedRoleAssignment](../resources/privilegedroleassignment.md)|Add assignments by posting to the assignments collection.|
|[Remove assignments](../api/privilegedrole-delete-assignments.md)|None|Remove an [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.|
|[List summary](../api/privilegedrole-list-summary.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md) collection|Get the privilegedRoleSummaries from the summary navigation property.|
|[Create summary](../api/privilegedrole-post-summary.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Create a new summary object.|
|[Delete summary](../api/privilegedrole-delete-summary.md)|None|Delete a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|
|[Update summary](../api/privilegedrole-update-summary.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Update the properties of a summary object.|
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md)|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|Read the properties and relationships of a [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection|**TODO: Add Description**|
|settings|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|**TODO: Add Description**|
|summary|[privilegedRoleSummary](../resources/privilegedrolesummary.md)|**TODO: Add Description**|

## JSON representation
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

