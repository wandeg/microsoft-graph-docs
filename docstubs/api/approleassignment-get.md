---
title: "Get appRoleAssignment"
description: "Read properties and relationships of an appRoleAssignment object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get appRoleAssignment

Namespace: microsoft.graph

Read properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.

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
GET /appRoleAssignments/{appRoleAssignmentsId}
GET /groups/{groupsId}/appRoleAssignments/{appRoleAssignmentId}
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo/{appRoleAssignmentId}
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignments/{appRoleAssignmentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/appRoleAssignments/{appRoleAssignmentsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.appRoleAssignment",
    "id": "c8a8540a-540a-c8a8-0a54-a8c80a54a8c8",
    "appRoleId": "f4770b24-0b24-f477-240b-77f4240b77f4",
    "creationTimestamp": "2017-01-01T00:03:07.5865287+03:00",
    "principalDisplayName": "Principal Display Name value",
    "principalId": "41836c63-6c63-4183-636c-8341636c8341",
    "principalType": "Principal Type value",
    "resourceDisplayName": "Resource Display Name value",
    "resourceId": "57fafaf0-faf0-57fa-f0fa-fa57f0fafa57"
  }
}
```

