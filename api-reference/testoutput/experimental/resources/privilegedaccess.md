---
title: "privilegedAccess resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# privilegedAccess resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedAccesses](../api/privilegedaccess-list.md)|[privilegedAccess](../resources/privilegedaccess.md) collection|List properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) objects.|
|[Get privilegedAccess](../api/privilegedaccess-get.md)|[privilegedAccess](../resources/privilegedaccess.md)|Read properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) object.|
|[Create privilegedAccess](../api/privilegedaccess-post-privilegedaccess.md)|[privilegedAccess](../resources/privilegedaccess.md)|Create a new [privilegedAccess](../resources/privilegedaccess.md) object.|
|[Delete privilegedAccess](../api/privilegedaccess-delete.md)|None|Deletes a [privilegedAccess](../resources/privilegedaccess.md).|
|[Update privilegedAccess](../api/privilegedaccess-update.md)|[privilegedAccess](../resources/privilegedaccess.md)|Update the properties of a [privilegedAccess](../resources/privilegedaccess.md) object.|
|[List resources](../api/privilegedaccess-list-resources.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resources navigation property.|
|[Add resources](../api/privilegedaccess-post-resources.md)|[governanceResource](../resources/governanceresource.md)|Add resources by posting to the resources collection.|
|[List roleDefinitions](../api/privilegedaccess-list-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/privilegedaccess-post-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/privilegedaccess-list-roleassignments.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection|Get the governanceRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/privilegedaccess-post-roleassignments.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleAssignmentRequests](../api/privilegedaccess-list-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection|Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.|
|[Add roleAssignmentRequests](../api/privilegedaccess-post-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Add roleAssignmentRequests by posting to the roleAssignmentRequests collection.|
|[List roleSettings](../api/privilegedaccess-list-rolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md) collection|Get the governanceRoleSettings from the roleSettings navigation property.|
|[Add roleSettings](../api/privilegedaccess-post-rolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Add roleSettings by posting to the roleSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resources|[governanceResource](../resources/governanceresource.md) collection||
|roleAssignmentRequests|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection||
|roleAssignments|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection||
|roleDefinitions|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection||
|roleSettings|[governanceRoleSetting](../resources/governancerolesetting.md) collection||

## JSON representation
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

