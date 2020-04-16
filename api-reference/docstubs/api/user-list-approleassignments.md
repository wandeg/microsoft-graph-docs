---
title: "List appRoleAssignments"
description: "Get the appRoleAssignments from the appRoleAssignments navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appRoleAssignments

Namespace: microsoft.graph

Get the appRoleAssignments from the appRoleAssignments navigation property.

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
GET /me/appRoleAssignments
GET /users/{usersId}/appRoleAssignments
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/appRoleAssignments
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appRoleAssignment",
      "id": "c448aa3f-aa3f-c448-3faa-48c43faa48c4",
      "appRoleId": "d44c275e-275e-d44c-5e27-4cd45e274cd4",
      "creationTimestamp": "2016-12-31T23:56:32.9939744+03:00",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "de51d196-d196-de51-96d1-51de96d151de",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "6046e9cf-e9cf-6046-cfe9-4660cfe94660"
    }
  ]
}
```

