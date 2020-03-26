---
title: "my"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# my

Namespace: microsoft.graph



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
GET /privilegedRoleAssignmentRequests/my
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
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
Content-Length: 664

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
      "id": "ee118416-8416-ee11-1684-11ee168411ee",
      "schedule": {
        "@odata.type": "microsoft.graph.governanceSchedule"
      },
      "userId": "User Id value",
      "roleId": "Role Id value",
      "type": "Type value",
      "assignmentState": "Assignment State value",
      "requestedDateTime": "2016-12-31T23:57:33.8345821+03:00",
      "status": "Status value",
      "duration": "Duration value",
      "reason": "Reason value",
      "ticketNumber": "Ticket Number value",
      "ticketSystem": "Ticket System value"
    }
  ]
}
```

