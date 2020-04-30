---
title: "List appRoleAssignments"
description: "Get a list of the appRoleAssignment objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List appRoleAssignments

Namespace: Microsoft.DirectoryServices

Get a list of the [appRoleAssignment](../resources/approleassignment.md) objects and their properties.

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
GET /appRoleAssignments
GET /me/appRoleAssignments
GET /users/{usersId}/appRoleAssignments
GET /groups/{groupsId}/appRoleAssignments
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignments
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
GET https://graph.microsoft.com/changelog/appRoleAssignments
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.approleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.appRoleAssignment",
      "appRoleId": "27bd2e88-2e88-27bd-882e-bd27882ebd27",
      "creationTimestamp": "2016-12-31T23:58:27.73127+00:00",
      "id": "32a22532-2532-32a2-3225-a2323225a232",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "0279f1dc-f1dc-0279-dcf1-7902dcf17902",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "95df367a-367a-95df-7a36-df957a36df95"
    }
  ]
}
```

