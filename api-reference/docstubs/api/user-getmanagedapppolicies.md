---
title: "user: getManagedAppPolicies"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getManagedAppPolicies

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/getManagedAppPolicies
GET /users/{usersId}/getManagedAppPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/managedapppolicy.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_getmanagedapppolicies"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getManagedAppPolicies
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedapppolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "id": "fc7b9743-9743-fc7b-4397-7bfc43977bfc",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "version": "Version value"
    }
  ]
}
```

