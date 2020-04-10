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
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "caa99f32-9f32-caa9-329f-a9ca329fa9ca",
      "schedule": {
        "@odata.type": "microsoft.graph.governanceSchedule",
        "type": "Type value",
        "startDateTime": "2016-12-31T23:57:39.2677321+00:00",
        "endDateTime": "2017-01-01T00:02:08.1909286+00:00",
        "duration": "-PT2M44.7705843S"
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
  ]
}
```

