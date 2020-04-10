---
title: "privilegedRoleAssignmentRequest: cancel"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# cancel

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
POST /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/cancel
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/cancel
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignmentrequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
    "id": "caa99f32-9f32-caa9-329f-a9ca329fa9ca",
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule"
    },
    "userId": "User Id value",
    "roleId": "Role Id value",
    "type": "Type value",
    "assignmentState": "Assignment State value",
    "requestedDateTime": "2016-12-31T23:57:01.4951864+00:00",
    "status": "Status value",
    "duration": "Duration value",
    "reason": "Reason value",
    "ticketNumber": "Ticket Number value",
    "ticketSystem": "Ticket System value"
  }
}
```

