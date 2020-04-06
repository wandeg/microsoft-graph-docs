---
title: "List appRoleAssignments"
description: "Get the appRoleAssignments from the appRoleAssignments navigation property."
author: ""
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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/appRoleAssignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
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
  ]
}
```

