---
title: "governanceResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# governanceResource resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceResource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Delete governanceResource](../api/governanceresource-delete.md)|None|Deletes a [governanceResource](../resources/governanceresource.md).|
|[Update governanceResource](../api/governanceresource-update.md)|[governanceResource](../resources/governanceResource.md)|Update the properties of a [governanceResource](../resources/governanceresource.md) object.|
|[register](../api/governanceresource-register.md)|None||
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceResource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[List roleDefinitions](../api/governanceresource-list-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/governanceresource-post-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceRoleDefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/governanceresource-list-roleassignments.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md) collection|Get the governanceRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/governanceresource-post-roleassignments.md)|[governanceRoleAssignment](../resources/governanceRoleAssignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleAssignmentRequests](../api/governanceresource-list-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md) collection|Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.|
|[Add roleAssignmentRequests](../api/governanceresource-post-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md)|Add roleAssignmentRequests by posting to the roleAssignmentRequests collection.|
|[List roleSettings](../api/governanceresource-list-rolesettings.md)|[governanceRoleSetting](../resources/governanceRoleSetting.md) collection|Get the governanceRoleSettings from the roleSettings navigation property.|
|[Add roleSettings](../api/governanceresource-post-rolesettings.md)|[governanceRoleSetting](../resources/governanceRoleSetting.md)|Add roleSettings by posting to the roleSettings collection.|
|[List resources](../api/privilegedaccess-list-resources.md)|[governanceResource](../resources/governanceResource.md) collection|Get the governanceResources from the resources navigation property.|
|[Add resources](../api/privilegedaccess-post-resources.md)|[governanceResource](../resources/governanceResource.md)|Add resources by posting to the resources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|registeredDateTime|DateTimeOffset||
|registeredRoot|String||
|status|String||
|type|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parent|[governanceResource](../resources/governanceResource.md)||
|roleAssignmentRequests|[governanceRoleAssignmentRequest](../resources/governanceRoleAssignmentRequest.md) collection||
|roleAssignments|[governanceRoleAssignment](../resources/governanceRoleAssignment.md) collection||
|roleDefinitions|[governanceRoleDefinition](../resources/governanceRoleDefinition.md) collection||
|roleSettings|[governanceRoleSetting](../resources/governanceRoleSetting.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceResource",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceResource",
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String"
}
```

