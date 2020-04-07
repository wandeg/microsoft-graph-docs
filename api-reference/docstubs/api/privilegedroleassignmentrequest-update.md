---
title: "Update privilegedRoleAssignmentRequest"
description: "Update the properties of a privilegedRoleAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedRoleAssignmentRequest

Namespace: microsoft.graph

Update the properties of a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

The following table shows the properties that are required when you create the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|schedule|[governanceSchedule](../resources/governanceschedule.md)||
|userId|String||
|roleId|String||
|type|String||
|assignmentState|String||
|requestedDateTime|DateTimeOffset||
|status|String||
|duration|String||
|reason|String||
|ticketNumber|String||
|ticketSystem|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedroleassignmentrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}
Content-type: application/json
Content-length: 700

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2016-12-31T23:57:07.1037922+03:00",
    "endDateTime": "2016-12-31T23:57:36.8091086+03:00",
    "duration": "PT2M30.816588S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:02:32.8728478+03:00",
  "status": "Status value",
  "duration": "Duration value",
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 749

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "id": "e7edc65e-c65e-e7ed-5ec6-ede75ec6ede7",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2016-12-31T23:57:07.1037922+03:00",
    "endDateTime": "2016-12-31T23:57:36.8091086+03:00",
    "duration": "PT2M30.816588S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:02:32.8728478+03:00",
  "status": "Status value",
  "duration": "Duration value",
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

