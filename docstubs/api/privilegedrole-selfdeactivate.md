---
title: "selfDeactivate"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# selfDeactivate

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
POST /privilegedRoles/{privilegedRolesId}/selfDeactivate
POST /privilegedApproval/{privilegedApprovalId}/roleInfo/selfDeactivate
POST /privilegedApproval/{privilegedApprovalId}/request/roleInfo/selfDeactivate
POST /privilegedRoleAssignments/{privilegedRoleAssignmentsId}/roleInfo/selfDeactivate
POST /privilegedRoleAssignmentRequests/{privilegedRoleAssignmentRequestsId}/roleInfo/selfDeactivate
POST /privilegedRoles/{privilegedRolesId}/assignments/{privilegedRoleAssignmentId}/roleInfo/selfDeactivate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/selfDeactivate
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
    "id": "f3fdf5d6-f5d6-f3fd-d6f5-fdf3d6f5fdf3",
    "userId": "User Id value",
    "roleId": "Role Id value",
    "isElevated": true,
    "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00",
    "resultMessage": "Result Message value"
  }
}
```

