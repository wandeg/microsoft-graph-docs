---
title: "privilegedApproval resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedApproval resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List privilegedApprovals](../api/privilegedapproval-list.md)|[privilegedApproval](../resources/privilegedapproval.md) collection|Get a list of the [privilegedApproval](../resources/privilegedapproval.md) objects and their properties.|
|[Get privilegedApproval](../api/privilegedapproval-get.md)|[privilegedApproval](../resources/privilegedapproval.md)|Read the properties and relationships of a [privilegedApproval](../resources/privilegedapproval.md) object.|
|[Create privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md)|[privilegedApproval](../resources/privilegedapproval.md)|Create a new [privilegedApproval](../resources/privilegedapproval.md) object.|
|[Delete privilegedApproval](../api/privilegedapproval-delete.md)|None|Deletes a [privilegedApproval](../resources/privilegedapproval.md) object.|
|[Update privilegedApproval](../api/privilegedapproval-update.md)|[privilegedApproval](../resources/privilegedapproval.md)|Update the properties of a [privilegedApproval](../resources/privilegedapproval.md) object.|
|[myRequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](../resources/privilegedapproval.md) collection|**TODO: Add Description**|
|[List request](../api/privilegedapproval-list-request.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection|Get the privilegedRoleAssignmentRequests from the request navigation property.|
|[Add request](../api/privilegedapproval-post-request.md)|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|Add request by posting to the request collection.|
|[Remove request](../api/privilegedapproval-delete-request.md)|None|Remove a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[List roleInfo](../api/privilegedapproval-list-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md) collection|Get the privilegedRoles from the roleInfo navigation property.|
|[Create roleInfo](../api/privilegedapproval-post-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Create a new roleInfo object.|
|[Delete roleInfo](../api/privilegedapproval-delete-roleinfo.md)|None|Delete a [privilegedRole](../resources/privilegedrole.md) object.|
|[Update roleInfo](../api/privilegedapproval-update-roleinfo.md)|[privilegedRole](../resources/privilegedrole.md)|Update the properties of a roleInfo object.|
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedrole.md)|Read the properties and relationships of a [privilegedRole](../resources/privilegedrole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalDuration|Duration|**TODO: Add Description**|
|approvalState|approvalState|**TODO: Add Description**. Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|String|**TODO: Add Description**|
|approverReason|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|requestorReason|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|request|[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)|**TODO: Add Description**|
|roleInfo|[privilegedRole](../resources/privilegedrole.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedApproval",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedApproval",
  "id": "String (identifier)",
  "userId": "String",
  "roleId": "String",
  "approvalType": "String",
  "approvalState": "String",
  "approvalDuration": "String (duration)",
  "requestorReason": "String",
  "approverReason": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

