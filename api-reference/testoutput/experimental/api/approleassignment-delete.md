---
title: "Delete appRoleAssignment"
description: "Deletes a appRoleAssignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete appRoleAssignment

Deletes a [appRoleAssignment](../resources/approleassignment.md).

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
DELETE /appRoleAssignments/{appRoleAssignmentsId}
DELETE /me/appRoleAssignments/{appRoleAssignmentId}
DELETE /users/{usersId}/appRoleAssignments/{appRoleAssignmentId}
DELETE /groups/{groupsId}/appRoleAssignments/{appRoleAssignmentId}
DELETE /me/joinedGroups/{groupId}/appRoleAssignments/{appRoleAssignmentId}
DELETE /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo/{appRoleAssignmentId}
DELETE /servicePrincipals/{servicePrincipalsId}/appRoleAssignments/{appRoleAssignmentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}
-->
``` http
DELETE https://graph.microsoft.com/docs\api/appRoleAssignments/{appRoleAssignmentsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

