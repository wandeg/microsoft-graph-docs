---
title: "List appRoleAssignments"
description: "List properties and relationships of the appRoleAssignment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appRoleAssignments

Namespace: microsoft.graph

List properties and relationships of the [appRoleAssignment](../resources/approleassignment.md) objects.

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
GET /appRoleAssignments
GET /me/appRoleAssignments
GET /users/{usersId}/appRoleAssignments
GET /groups/{groupsId}/appRoleAssignments
GET /me/joinedGroups/{groupId}/appRoleAssignments
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignments
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
If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/appRoleAssignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
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
  ]
}
```

