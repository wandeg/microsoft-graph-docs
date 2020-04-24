---
title: "Create appRoleAssignments"
description: "Create a new appRoleAssignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [appRoleAssignment](../resources/approleassignment.md) object.

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
Content-length: 450

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "497abf4a-bf4a-497a-4abf-7a494abf7a49",
  "creationTimestamp": "2016-12-31T23:58:14.554254+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "8465fac1-fac1-8465-c1fa-6584c1fa6584",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "d4b1a5c2-a5c2-d4b1-c2a5-b1d4c2a5b1d4"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
  "id": "f6cde9bb-e9bb-f6cd-bbe9-cdf6bbe9cdf6",
  "appRoleId": "497abf4a-bf4a-497a-4abf-7a494abf7a49",
  "creationTimestamp": "2016-12-31T23:58:14.554254+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "8465fac1-fac1-8465-c1fa-6584c1fa6584",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "d4b1a5c2-a5c2-d4b1-c2a5-b1d4c2a5b1d4"
}
```

