---
title: "privilegedRoleAssignmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedRoleAssignmentRequest resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List request](../api/privilegedapproval-list-request.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection|Get the privilegedRoleAssignmentRequests from the request navigation property.|
|[Add request](../api/privilegedapproval-post-request.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Add request by posting to the request collection.|
|[Remove request](../api/privilegedapproval-delete-request.md)|None|Remove a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[List privilegedRoleAssignmentRequests](../api/privilegedroleassignmentrequest-list.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection|Get a list of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects and their properties.|
|[Create privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-post-privilegedroleassignmentrequests.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Create a new [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Get privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-get.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Read the properties and relationships of a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Update privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-update.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Update the properties of a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Delete privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-delete.md)|None|Deletes a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[my](../api/privilegedroleassignmentrequest-my.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection|**TODO: Add Description**|
|[cancel](../api/privilegedroleassignmentrequest-cancel.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|**TODO: Add Description**|
|[List roleInfo](../api/privilegedroleassignmentrequest-list-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md) collection|Get the privilegedRoles from the roleInfo navigation property.|
|[Create roleInfo](../api/privilegedroleassignmentrequest-post-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Create a new roleInfo object.|
|[Get roleInfo](../api/privilegedroleassignmentrequest-get-privilegedrole.md)|[privilegedRole](../resources/privilegedrole.md)|Read the properties and relationships of a [privilegedRole](../resources/privilegedrole.md) object.|
|[Update roleInfo](../api/privilegedroleassignmentrequest-update-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Update the properties of a roleInfo object.|
|[Delete roleInfo](../api/privilegedroleassignmentrequest-delete-roleinfo.md)|None|Delete a [privilegedRole](../resources/privilegedrole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String|**TODO: Add Description**|
|duration|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reason|String|**TODO: Add Description**|
|requestedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|ticketNumber|String|**TODO: Add Description**|
|ticketSystem|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
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
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "id": "String (identifier)",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule"
  },
  "userId": "String",
  "roleId": "String",
  "type": "String",
  "assignmentState": "String",
  "requestedDateTime": "String (timestamp)",
  "status": "String",
  "duration": "String",
  "reason": "String",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

