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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privilegedRoleAssignmentRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/privilegedRoleAssignmentRequests
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
Content-Length: 860

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
      "id": "4eb017cd-17cd-4eb0-cd17-b04ecd17b04e",
      "schedule": {
        "@odata.type": "microsoft.graph.governanceSchedule",
        "type": "Type value",
        "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
        "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
        "duration": "-PT1M55.0810357S"
      },
      "userId": "User Id value",
      "roleId": "Role Id value",
      "type": "Type value",
      "assignmentState": "Assignment State value",
      "requestedDateTime": "2017-01-01T00:02:43.4981192+03:00",
      "status": "Status value",
      "duration": "Duration value",
      "reason": "Reason value",
      "ticketNumber": "Ticket Number value",
      "ticketSystem": "Ticket System value"
    }
  ]
}
```

