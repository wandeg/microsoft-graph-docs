---
title: "privilegedAccess resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedAccess resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedAccesses](../api/privilegedaccess-list.md)|[privilegedAccess](../resources/privilegedAccess.md) collection|List properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) objects.|
|[Get privilegedAccess](../api/privilegedaccess-get.md)|[privilegedAccess](../resources/privilegedAccess.md)|Read properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) object.|
|[Create privilegedAccess](../api/privilegedaccess-post-privilegedaccess.md)|[privilegedAccess](../resources/privilegedAccess.md)|Create a new [privilegedAccess](../resources/privilegedaccess.md) object.|
|[Delete privilegedAccess](../api/privilegedaccess-delete.md)|None|Deletes a [privilegedAccess](../resources/privilegedaccess.md).|
|[Update privilegedAccess](../api/privilegedaccess-update.md)|[privilegedAccess](../resources/privilegedAccess.md)|Update the properties of a [privilegedAccess](../resources/privilegedaccess.md) object.|
|[List resources](../api/privilegedaccess-list-resources.md)|[governanceResource](../resources/governanceResource.md) collection|Get the governanceResources from the resources navigation property.|
|[Add resources](../api/privilegedaccess-post-resources.md)|[governanceResource](../resources/governanceResource.md)|Add resources by posting to the resources collection.|
|[List roleDefinitions](../api/privilegedaccess-list-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/privilegedaccess-post-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/privilegedaccess-list-roleassignments.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md) collection|Get the governanceRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/privilegedaccess-post-roleassignments.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleAssignmentRequests](../api/privilegedaccess-list-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md) collection|Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.|
|[Add roleAssignmentRequests](../api/privilegedaccess-post-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md)|Add roleAssignmentRequests by posting to the roleAssignmentRequests collection.|
|[List roleSettings](../api/privilegedaccess-list-rolesettings.md)|[governanceRoleSetting](../resources/governanceRoleSetting.md) collection|Get the governanceRoleSettings from the roleSettings navigation property.|
|[Add roleSettings](../api/privilegedaccess-post-rolesettings.md)|[governanceRoleSetting](../resources/governanceRoleSetting.md)|Add roleSettings by posting to the roleSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resources|[governanceResource](../resources/governanceResource.md) collection||
|roleAssignmentRequests|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md) collection||
|roleAssignments|[governanceRoleAssignment](../resources/governanceRoleAssignment.md) collection||
|roleDefinitions|[governanceRoleDefinition](../resources/governanceRoleDefinition.md) collection||
|roleSettings|[governanceRoleSetting](../resources/governanceRoleSetting.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedAccess",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedAccess",
  "id": "String (identifier)",
  "displayName": "String"
}
```

