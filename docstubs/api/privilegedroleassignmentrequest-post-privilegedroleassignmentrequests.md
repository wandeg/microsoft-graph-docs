---
title: "Create privilegedRoleAssignmentRequest"
description: "Create a new privilegedRoleAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedRoleAssignmentRequest

Namespace: microsoft.graph

Create a new [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

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
POST /privilegedRoleAssignmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignmentrequest_from_privilegedroleassignmentrequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json
Content-length: 700

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2016-12-31T23:57:40.5444496+00:00",
    "endDateTime": "2016-12-31T23:58:47.51829+00:00",
    "duration": "-PT2M12.8464123S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:02:08.4080349+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 749

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
  "id": "2e2e06cd-06cd-2e2e-cd06-2e2ecd062e2e",
  "schedule": {
    "@odata.type": "microsoft.graph.governanceSchedule",
    "type": "Type value",
    "startDateTime": "2016-12-31T23:57:40.5444496+00:00",
    "endDateTime": "2016-12-31T23:58:47.51829+00:00",
    "duration": "-PT2M12.8464123S"
  },
  "userId": "User Id value",
  "roleId": "Role Id value",
  "type": "Type value",
  "assignmentState": "Assignment State value",
  "requestedDateTime": "2017-01-01T00:02:08.4080349+00:00",
  "status": "Status value",
  "duration": "Duration value",
  "reason": "Reason value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

