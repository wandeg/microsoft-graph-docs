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
GET /groups/{groupsId}/appRoleAssignments
GET /me/joinedGroups/{groupId}/appRoleAssignments
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
GET https://graph.microsoft.com/beta/groups/{groupsId}/appRoleAssignments
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
      "id": "0bee30f9-30f9-0bee-f930-ee0bf930ee0b",
      "appRoleId": "162f4de6-4de6-162f-e64d-2f16e64d2f16",
      "creationTimestamp": "2017-01-01T00:02:21.1717664+03:00",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "542b7c28-7c28-542b-287c-2b54287c2b54",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "c5a6a24f-a24f-c5a6-4fa2-a6c54fa2a6c5"
    }
  ]
}
```

