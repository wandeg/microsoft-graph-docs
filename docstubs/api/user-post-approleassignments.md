---
title: "Create appRoleAssignments"
description: "Create a new appRoleAssignments object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create appRoleAssignments

Namespace: microsoft.graph

Create a new appRoleAssignments object.

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
POST /me/appRoleAssignments
POST /users/{usersId}/appRoleAssignments
POST /invitations/{invitationsId}/invitedUser/appRoleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [appRoleAssignment](../resources/approleassignment.md) object.

The following table shows the properties that are required when you create the [appRoleAssignment](../resources/approleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appRoleId|Guid|**TODO: Add Description**|
|creationTimestamp|DateTimeOffset|**TODO: Add Description**|
|principalDisplayName|String|**TODO: Add Description**|
|principalId|Guid|**TODO: Add Description**|
|principalType|String|**TODO: Add Description**|
|resourceDisplayName|String|**TODO: Add Description**|
|resourceId|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_approleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/appRoleAssignments
Content-Type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "f4770b24-0b24-f477-240b-77f4240b77f4",
  "creationTimestamp": "2017-01-01T00:03:07.5865287+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "41836c63-6c63-4183-636c-8341636c8341",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "57fafaf0-faf0-57fa-f0fa-fa57f0fafa57"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

