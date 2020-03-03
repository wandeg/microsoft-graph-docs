---
title: "selfActivate"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# selfActivate

Namespace: microsoft.graph



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
POST /privilegedRoles/{privilegedRolesId}/selfActivate
POST /privilegedApproval/{privilegedApprovalId}/roleInfo/selfActivate
POST /privilegedApproval/{privilegedApprovalId}/request/roleInfo/selfActivate
POST /privilegedRoleAssignments/{privilegedRoleAssignmentsId}/roleInfo/selfActivate
POST /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/roleInfo/selfActivate
POST /privilegedRoles/{privilegedRolesId}/assignments/{privilegedRoleAssignmentId}/roleInfo/selfActivate
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|reason|String||
|duration|String||
|ticketNumber|String||
|ticketSystem|String||



## Response
If successful, this action returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}
-->
``` http
POST https://graph.microsoft.com/localtest/privilegedRoles/{privilegedRolesId}/selfActivate

Content-type: application/json
Content-length: 149

{
  "reason": "Reason value",
  "duration": "Duration value",
  "ticketNumber": "Ticket Number value",
  "ticketSystem": "Ticket System value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 337

{
  "value": {
    "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
    "id": "59a88cae-8cae-59a8-ae8c-a859ae8ca859",
    "userId": "User Id value",
    "roleId": "Role Id value",
    "isElevated": true,
    "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
    "resultMessage": "Result Message value"
  }
}
```

