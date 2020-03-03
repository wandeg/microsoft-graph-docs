---
title: "Get appRoleAssignment"
description: "Read properties and relationships of the appRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get appRoleAssignment

Read properties and relationships of the [appRoleAssignment](../resources/approleassignment.md) object.

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
GET /appRoleAssignments/{appRoleAssignmentsId}
GET /me/appRoleAssignments/{appRoleAssignmentId}
GET /users/{usersId}/appRoleAssignments/{appRoleAssignmentId}
GET /groups/{groupsId}/appRoleAssignments/{appRoleAssignmentId}
GET /me/joinedGroups/{groupId}/appRoleAssignments/{appRoleAssignmentId}
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo/{appRoleAssignmentId}
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignments/{appRoleAssignmentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/appRoleAssignments/{appRoleAssignmentsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 537

{
  "value": {
    "@odata.type": "#microsoft.graph.appRoleAssignment",
    "id": "110e998a-998a-110e-8a99-0e118a990e11",
    "appRoleId": "d105223c-223c-d105-3c22-05d13c2205d1",
    "creationTimestamp": "2017-01-01T00:03:08.4498325+03:00",
    "principalDisplayName": "Principal Display Name value",
    "principalId": "ad7e366f-366f-ad7e-6f36-7ead6f367ead",
    "principalType": "Principal Type value",
    "resourceDisplayName": "Resource Display Name value",
    "resourceId": "05450f46-0f46-0545-460f-4505460f4505"
  }
}
```

