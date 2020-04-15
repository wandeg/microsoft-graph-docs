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
GET /groups/{groupsId}/appRoleAssignments
GET /me/joinedGroups/{groupId}/appRoleAssignments
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
GET https://graph.microsoft.com/beta/groups/{groupsId}/appRoleAssignments
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
      "id": "aa82cd1c-cd1c-aa82-1ccd-82aa1ccd82aa",
      "appRoleId": "d9399ecd-9ecd-d939-cd9e-39d9cd9e39d9",
      "creationTimestamp": "2017-01-01T00:03:32.8125718+03:00",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "5e973e8a-3e8a-5e97-8a3e-975e8a3e975e",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "839bba7c-ba7c-839b-7cba-9b837cba9b83"
    }
  ]
}
```

