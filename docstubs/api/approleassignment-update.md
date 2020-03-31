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
Content-length: 450

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "2796e42c-e42c-2796-2ce4-96272ce49627",
  "creationTimestamp": "2016-12-31T23:56:32.946064+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "cbd81be4-1be4-cbd8-e41b-d8cbe41bd8cb",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "1ff768af-68af-1ff7-af68-f71faf68f71f"
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
Content-Length: 499

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "7f8c04ac-04ac-7f8c-ac04-8c7fac048c7f",
  "appRoleId": "2796e42c-e42c-2796-2ce4-96272ce49627",
  "creationTimestamp": "2016-12-31T23:56:32.946064+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "cbd81be4-1be4-cbd8-e41b-d8cbe41bd8cb",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "1ff768af-68af-1ff7-af68-f71faf68f71f"
}
```

