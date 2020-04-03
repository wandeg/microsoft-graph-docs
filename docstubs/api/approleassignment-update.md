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
  "appRoleId": "63373109-3109-6337-0931-376309313763",
  "creationTimestamp": "2016-12-31T23:56:55.872626+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3c0b18e9-18e9-3c0b-e918-0b3ce9180b3c",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "41c49f25-9f25-41c4-259f-c441259fc441"
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
  "id": "3ca445ac-45ac-3ca4-ac45-a43cac45a43c",
  "appRoleId": "63373109-3109-6337-0931-376309313763",
  "creationTimestamp": "2016-12-31T23:56:55.872626+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3c0b18e9-18e9-3c0b-e918-0b3ce9180b3c",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "41c49f25-9f25-41c4-259f-c441259fc441"
}
```

