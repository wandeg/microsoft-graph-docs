---
title: "List privilegedRoleAssignmentRequests"
description: "List properties and relationships of the privilegedRoleAssignmentRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedRoleAssignmentRequests

Namespace: microsoft.graph

List properties and relationships of the [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects.

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
GET /privilegedRoleAssignmentRequests
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
If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedroleassignmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
      "id": "1859fce8-fce8-1859-e8fc-5918e8fc5918",
      "schedule": {
        "@odata.type": "microsoft.graph.governanceSchedule",
        "type": "Type value",
        "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
        "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
        "duration": "PT1M50.4113871S"
      },
      "userId": "User Id value",
      "roleId": "Role Id value",
      "type": "Type value",
      "assignmentState": "Assignment State value",
      "requestedDateTime": "2017-01-01T00:00:43.619433+03:00",
      "status": "Status value",
      "duration": "Duration value",
      "reason": "Reason value",
      "ticketNumber": "Ticket Number value",
      "ticketSystem": "Ticket System value"
    }
  ]
}
```

