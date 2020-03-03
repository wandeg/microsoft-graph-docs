---
title: "privilegedApproval resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedApproval resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedApprovals](../api/privilegedapproval-list.md)|[privilegedApproval](../resources/privilegedApproval.md) collection|List properties and relationships of the [privilegedApproval](../resources/privilegedapproval.md) objects.|
|[Get privilegedApproval](../api/privilegedapproval-get.md)|[privilegedApproval](../resources/privilegedApproval.md)|Read properties and relationships of the [privilegedApproval](../resources/privilegedapproval.md) object.|
|[Create privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md)|[privilegedApproval](../resources/privilegedApproval.md)|Create a new [privilegedApproval](../resources/privilegedapproval.md) object.|
|[Delete privilegedApproval](../api/privilegedapproval-delete.md)|None|Deletes a [privilegedApproval](../resources/privilegedapproval.md).|
|[Update privilegedApproval](../api/privilegedapproval-update.md)|[privilegedApproval](../resources/privilegedApproval.md)|Update the properties of a [privilegedApproval](../resources/privilegedapproval.md) object.|
|[myRequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](../resources/privilegedApproval.md) collection||
|[Get privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-get.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)|Read properties and relationships of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedRole.md)|Read properties and relationships of the [privilegedRole](../resources/privilegedrole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalDuration|Duration||
|approvalState|Enumeration|. Possible values are: `pending`, `approved`, `denied`, `aborted`, `canceled`.|
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset||
|userId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|request|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)||
|roleInfo|[privilegedRole](../resources/privilegedRole.md)||

## JSON Representation
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

