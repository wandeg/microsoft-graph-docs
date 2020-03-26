---
title: "Get scopedRoleMembership"
description: "Read properties and relationships of the scopedRoleMembership object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get scopedRoleMembership

Namespace: microsoft.graph

Read properties and relationships of the [scopedRoleMembership](../resources/scopedrolemembership.md) object.

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
GET /me/scopedRoleMemberOf/{scopedRoleMembershipId}
GET /scopedRoleMemberships/{scopedRoleMembershipsId}
GET /users/{usersId}/scopedRoleMemberOf/{scopedRoleMembershipId}
GET /directoryRoles/{directoryRolesId}/scopedMembers/{scopedRoleMembershipId}
GET /administrativeUnits/{administrativeUnitsId}/scopedRoleMembers/{scopedRoleMembershipId}
GET /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/scopedRoleMembers/{scopedRoleMembershipId}
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
If successful, this method returns a `200 OK` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemembership"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf/{scopedRoleMembershipId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 378

{
  "value": {
    "@odata.type": "#microsoft.graph.scopedRoleMembership",
    "id": "8aa4858a-858a-8aa4-8a85-a48a8a85a48a",
    "roleId": "Role Id value",
    "administrativeUnitId": "Administrative Unit Id value",
    "roleMemberInfo": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  }
}
```

