---
title: "governanceResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceResource resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceResources](../api/governanceresource-list.md)|[governanceResource](../resources/governanceresource.md) collection|List properties and relationships of the [governanceResource](../resources/governanceresource.md) objects.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[Create governanceResource](../api/governanceresource-post-governanceresources.md)|[governanceResource](../resources/governanceresource.md)|Create a new [governanceResource](../resources/governanceresource.md) object.|
|[Delete governanceResource](../api/governanceresource-delete.md)|None|Deletes a [governanceResource](../resources/governanceresource.md).|
|[Update governanceResource](../api/governanceresource-update.md)|[governanceResource](../resources/governanceresource.md)|Update the properties of a [governanceResource](../resources/governanceresource.md) object.|
|[register](../api/governanceresource-register.md)|None||
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|
|[List roleDefinitions](../api/governanceresource-list-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection|Get the governanceRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/governanceresource-post-roledefinitions.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/governanceresource-list-roleassignments.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection|Get the governanceRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/governanceresource-post-roleassignments.md)|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Add roleAssignments by posting to the roleAssignments collection.|
|[List roleAssignmentRequests](../api/governanceresource-list-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection|Get the governanceRoleAssignmentRequests from the roleAssignmentRequests navigation property.|
|[Add roleAssignmentRequests](../api/governanceresource-post-roleassignmentrequests.md)|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Add roleAssignmentRequests by posting to the roleAssignmentRequests collection.|
|[List roleSettings](../api/governanceresource-list-rolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md) collection|Get the governanceRoleSettings from the roleSettings navigation property.|
|[Add roleSettings](../api/governanceresource-post-rolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Add roleSettings by posting to the roleSettings collection.|
|[List resources](../api/privilegedaccess-list-resources.md)|[governanceResource](../resources/governanceresource.md) collection|Get the governanceResources from the resources navigation property.|
|[Add resources](../api/privilegedaccess-post-resources.md)|[governanceResource](../resources/governanceresource.md)|Add resources by posting to the resources collection.|

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
|parent|[governanceResource](../resources/governanceresource.md)||
|roleAssignmentRequests|[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) collection||
|roleAssignments|[governanceRoleAssignment](../resources/governanceroleassignment.md) collection||
|roleDefinitions|[governanceRoleDefinition](../resources/governanceroledefinition.md) collection||
|roleSettings|[governanceRoleSetting](../resources/governancerolesetting.md) collection||

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

