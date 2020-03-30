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
  "appRoleId": "162f4de6-4de6-162f-e64d-2f16e64d2f16",
  "creationTimestamp": "2017-01-01T00:02:21.1717664+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "542b7c28-7c28-542b-287c-2b54287c2b54",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "c5a6a24f-a24f-c5a6-4fa2-a6c54fa2a6c5"
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
  "id": "0bee30f9-30f9-0bee-f930-ee0bf930ee0b",
  "appRoleId": "162f4de6-4de6-162f-e64d-2f16e64d2f16",
  "creationTimestamp": "2017-01-01T00:02:21.1717664+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "542b7c28-7c28-542b-287c-2b54287c2b54",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "c5a6a24f-a24f-c5a6-4fa2-a6c54fa2a6c5"
}
```

