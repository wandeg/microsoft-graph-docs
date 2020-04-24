---
title: "Create privilegedRoleAssignmentRequest"
description: "Create a new privilegedRoleAssignmentRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedRoleAssignmentRequest

Namespace: microsoft.graph

Create a new [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /privilegedRoleAssignmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

The following table shows the properties that are required when you create the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|schedule|[governanceSchedule](../resources/governanceschedule.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|assignmentState|String|**TODO: Add Description**|
|requestedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|duration|String|**TODO: Add Description**|
|reason|String|**TODO: Add Description**|
|ticketNumber|String|**TODO: Add Description**|
|ticketSystem|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignmentrequest_from_privilegedroleassignmentrequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-Type: application/json
Content-length: 699

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "duration": "-PT0.9940994S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:01:27.8869422+03:00",
  "status": "Status value",
  "duration": "Duration value",
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "id": "39d6a9f5-a9f5-39d6-f5a9-d639f5a9d639",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "duration": "-PT0.9940994S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:01:27.8869422+03:00",
  "status": "Status value",
  "duration": "Duration value",
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

