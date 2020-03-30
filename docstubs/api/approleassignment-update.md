---
title: "Update appRoleAssignment"
description: "Update the properties of a appRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update appRoleAssignment

Namespace: microsoft.graph

Update the properties of a [appRoleAssignment](../resources/approleassignment.md) object.

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
PATCH /appRoleAssignments/{appRoleAssignmentsId}
PATCH /me/appRoleAssignments/{appRoleAssignmentId}
PATCH /users/{usersId}/appRoleAssignments/{appRoleAssignmentId}
PATCH /groups/{groupsId}/appRoleAssignments/{appRoleAssignmentId}
PATCH /me/joinedGroups/{groupId}/appRoleAssignments/{appRoleAssignmentId}
PATCH /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo/{appRoleAssignmentId}
PATCH /servicePrincipals/{servicePrincipalsId}/appRoleAssignments/{appRoleAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [appRoleAssignment](../resources/approleassignment.md) object.

The following table shows the properties that are required when you create the [appRoleAssignment](../resources/approleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|appRoleId|Guid||
|creationTimestamp|DateTimeOffset||
|principalDisplayName|String||
|principalId|Guid||
|principalType|String||
|resourceDisplayName|String||
|resourceId|Guid||



## Response
If successful, this method returns a `200 OK` response code and an updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{appRoleAssignmentsId}
Content-type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "1103a398-a398-1103-98a3-031198a30311",
  "creationTimestamp": "2017-01-01T00:00:03.3963163+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "a01d40a7-40a7-a01d-a740-1da0a7401da0",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "12fe088d-088d-12fe-8d08-fe128d08fe12"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "782cc608-c608-782c-08c6-2c7808c62c78",
  "appRoleId": "1103a398-a398-1103-98a3-031198a30311",
  "creationTimestamp": "2017-01-01T00:00:03.3963163+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "a01d40a7-40a7-a01d-a740-1da0a7401da0",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "12fe088d-088d-12fe-8d08-fe128d08fe12"
}
```

