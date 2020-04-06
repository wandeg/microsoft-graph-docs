---
title: "Add appRoleAssignments"
description: "Add appRoleAssignments by posting to the appRoleAssignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appRoleAssignments

Namespace: microsoft.graph

Add appRoleAssignments by posting to the appRoleAssignments collection.

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
POST /me/appRoleAssignments/$ref
POST /users/{usersId}/appRoleAssignments/$ref
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
POST https://graph.microsoft.com/beta/me/appRoleAssignments
Content-type: application/json
Content-length: 451

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "9d79f96f-f96f-9d79-6ff9-799d6ff9799d",
  "creationTimestamp": "2017-01-01T00:02:44.7529688+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "fe4b246f-246f-fe4b-6f24-4bfe6f244bfe",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "02a18cce-8cce-02a1-ce8c-a102ce8ca102"
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
  "id": "bfc1b4e7-b4e7-bfc1-e7b4-c1bfe7b4c1bf",
  "appRoleId": "9d79f96f-f96f-9d79-6ff9-799d6ff9799d",
  "creationTimestamp": "2017-01-01T00:02:44.7529688+00:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "fe4b246f-246f-fe4b-6f24-4bfe6f244bfe",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "02a18cce-8cce-02a1-ce8c-a102ce8ca102"
}
```

