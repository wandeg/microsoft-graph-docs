---
title: "Create appRoleAssignment"
description: "Create a new appRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create appRoleAssignment

Namespace: microsoft.graph

Create a new [appRoleAssignment](../resources/approleassignment.md) object.

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
POST /appRoleAssignments
POST /me/appRoleAssignments
POST /users/{usersId}/appRoleAssignments
POST /groups/{groupsId}/appRoleAssignments
POST /me/joinedGroups/{groupId}/appRoleAssignments
POST /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
POST /servicePrincipals/{servicePrincipalsId}/appRoleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_approleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/appRoleAssignments
Content-type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "fd386795-6795-fd38-9567-38fd956738fd",
  "creationTimestamp": "2016-12-31T23:59:05.9293623+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "4f2ed7fb-d7fb-4f2e-fbd7-2e4ffbd72e4f",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "f937ce94-ce94-f937-94ce-37f994ce37f9"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "6b1523e7-23e7-6b15-e723-156be723156b",
  "appRoleId": "fd386795-6795-fd38-9567-38fd956738fd",
  "creationTimestamp": "2016-12-31T23:59:05.9293623+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "4f2ed7fb-d7fb-4f2e-fbd7-2e4ffbd72e4f",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "f937ce94-ce94-f937-94ce-37f994ce37f9"
}
```

