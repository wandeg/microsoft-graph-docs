---
title: "Get scopedRoleMembership"
description: "Read properties and relationships of a scopedRoleMembership object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get scopedRoleMembership

Namespace: Microsoft.DirectoryServices

Read properties and relationships of a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.

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
GET /me/scopedRoleMemberOf/{scopedRoleMembershipId}
GET /scopedRoleMemberships/{scopedRoleMembershipsId}
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
If successful, this method returns a `200 OK` response code and a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemembership"
}
-->
``` http
GET https://graph.microsoft.com/changelog/me/scopedRoleMemberOf/{scopedRoleMembershipId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.scopedRoleMembership"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.scopedRoleMembership",
    "id": "2a167424-7424-2a16-2474-162a2474162a",
    "roleId": "Role Id value",
    "administrativeUnitId": "Administrative Unit Id value",
    "roleMemberInfo": {
      "@odata.type": "Microsoft.DirectoryServices.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  }
}
```

