---
title: "privilegedRoleAssignmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedRoleAssignmentRequest resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoleAssignmentRequests](../api/privilegedroleassignmentrequest-list.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) collection|List properties and relationships of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects.|
|[Get privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-get.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)|Read properties and relationships of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Create privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-post-privilegedroleassignmentrequests.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)|Create a new [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[Delete privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-delete.md)|None|Deletes a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).|
|[Update privilegedRoleAssignmentRequest](../api/privilegedroleassignmentrequest-update.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)|Update the properties of a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.|
|[my](../api/privilegedroleassignmentrequest-my.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) collection||
|[cancel](../api/privilegedroleassignmentrequest-cancel.md)|[privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md)||
|[Get privilegedRole](../api/privilegedrole-get.md)|[privilegedRole](../resources/privilegedRole.md)|Read properties and relationships of the [privilegedRole](../resources/privilegedrole.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentState|String||
|duration|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|reason|String||
|requestedDateTime|DateTimeOffset||
|roleId|String||
|schedule|[governanceSchedule](../resources/governanceSchedule.md)||
|status|String||
|ticketNumber|String||
|ticketSystem|String||
|type|String||
|userId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleInfo|[privilegedRole](../resources/privilegedRole.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "String",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "duration": "String (duration)"
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

