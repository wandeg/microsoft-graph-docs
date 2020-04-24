---
title: "privilegedRoleAssignmentRequest: cancel"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# cancel

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/cancel
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignmentrequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleAssignmentRequest",
    "id": "39d6a9f5-a9f5-39d6-f5a9-d639f5a9d639",
    "schedule": {
      "@odata.type": "microsoft.graph.governanceSchedule"
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
}
```

