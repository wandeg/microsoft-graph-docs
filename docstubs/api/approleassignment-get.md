---
title: "Get appRoleAssignment"
description: "Read properties and relationships of the appRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get appRoleAssignment

Namespace: microsoft.graph

Read properties and relationships of the [appRoleAssignment](../resources/approleassignment.md) object.

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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/appRoleAssignments/{appRoleAssignmentsId}
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
Content-Length: 536

{
  "value": {
    "@odata.type": "#microsoft.graph.appRoleAssignment",
    "id": "3ca445ac-45ac-3ca4-ac45-a43cac45a43c",
    "appRoleId": "63373109-3109-6337-0931-376309313763",
    "creationTimestamp": "2016-12-31T23:56:55.872626+00:00",
    "principalDisplayName": "Principal Display Name value",
    "principalId": "3c0b18e9-18e9-3c0b-e918-0b3ce9180b3c",
    "principalType": "Principal Type value",
    "resourceDisplayName": "Resource Display Name value",
    "resourceId": "41c49f25-9f25-41c4-259f-c441259fc441"
  }
}
```

