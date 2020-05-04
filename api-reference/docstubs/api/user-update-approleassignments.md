---
title: "Update appRoleAssignments"
description: "Update the properties of an appRoleAssignments object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update appRoleAssignments

Namespace: microsoft.graph

Update the properties of an appRoleAssignments object.

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
PATCH /me/appRoleAssignments
PATCH /users/{usersId}/appRoleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_approleassignments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/appRoleAssignments
Content-Type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "4ef079cc-79cc-4ef0-cc79-f04ecc79f04e",
  "creationTimestamp": "2017-01-01T00:03:27.804947+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3bea14a8-14a8-3bea-a814-ea3ba814ea3b",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "76c2b97a-b97a-76c2-7ab9-c2767ab9c276"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "id": "7ab7b70b-b70b-7ab7-0bb7-b77a0bb7b77a",
  "appRoleId": "4ef079cc-79cc-4ef0-cc79-f04ecc79f04e",
  "creationTimestamp": "2017-01-01T00:03:27.804947+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "3bea14a8-14a8-3bea-a814-ea3ba814ea3b",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "76c2b97a-b97a-76c2-7ab9-c2767ab9c276"
}
```

