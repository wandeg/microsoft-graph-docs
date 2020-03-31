---
title: "Get privilegedRoleAssignmentRequest"
description: "Read properties and relationships of the privilegedRoleAssignmentRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get privilegedRoleAssignmentRequest

Namespace: microsoft.graph

Read properties and relationships of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object.

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
GET /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 805

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
    "id": "abe456f7-56f7-abe4-f756-e4abf756e4ab",
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule",
      "type": "Type value",
      "startDateTime": "2017-01-01T00:03:09.5259332+03:00",
      "endDateTime": "2016-12-31T23:57:04.2596185+03:00",
      "duration": "PT58.0389239S"
    },
    "userId": "User Id value",
    "roleId": "Role Id value",
    "type": "Type value",
    "assignmentState": "Assignment State value",
    "requestedDateTime": "2016-12-31T23:57:34.0011511+03:00",
    "status": "Status value",
    "duration": "Duration value",
    "reason": "Reason value",
    "ticketNumber": "Ticket Number value",
    "ticketSystem": "Ticket System value"
  }
}
```

