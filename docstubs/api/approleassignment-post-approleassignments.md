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
  "appRoleId": "77b80872-0872-77b8-7208-b8777208b877",
  "creationTimestamp": "2016-12-31T23:57:16.0977744+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3c579cd9-9cd9-3c57-d99c-573cd99c573c",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "332a07a3-07a3-332a-a307-2a33a3072a33"
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
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "85dc7c33-7c33-85dc-337c-dc85337cdc85",
  "appRoleId": "77b80872-0872-77b8-7208-b8777208b877",
  "creationTimestamp": "2016-12-31T23:57:16.0977744+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3c579cd9-9cd9-3c57-d99c-573cd99c573c",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "332a07a3-07a3-332a-a307-2a33a3072a33"
}
```

