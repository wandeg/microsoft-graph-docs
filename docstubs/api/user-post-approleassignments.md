---
title: "Add appRoleAssignments"
description: "Add appRoleAssignments by posting to the appRoleAssignments collection."
author: "**TODO: Provide Github Name**"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
  "appRoleId": "d9399ecd-9ecd-d939-cd9e-39d9cd9e39d9",
  "creationTimestamp": "2017-01-01T00:03:32.8125718+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "5e973e8a-3e8a-5e97-8a3e-975e8a3e975e",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "839bba7c-ba7c-839b-7cba-9b837cba9b83"
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
  "id": "aa82cd1c-cd1c-aa82-1ccd-82aa1ccd82aa",
  "appRoleId": "d9399ecd-9ecd-d939-cd9e-39d9cd9e39d9",
  "creationTimestamp": "2017-01-01T00:03:32.8125718+03:00",
  "principalDisplayName": "Principal Display Name value",
  "principalId": "5e973e8a-3e8a-5e97-8a3e-975e8a3e975e",
  "principalType": "Principal Type value",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "839bba7c-ba7c-839b-7cba-9b837cba9b83"
}
```

