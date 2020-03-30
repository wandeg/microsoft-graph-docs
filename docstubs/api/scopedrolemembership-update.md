---
title: "Update scopedRoleMembership"
description: "Update the properties of a scopedRoleMembership object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update scopedRoleMembership

Namespace: microsoft.graph

Update the properties of a [scopedRoleMembership](../resources/scopedrolemembership.md) object.

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
PATCH /me/scopedRoleMemberOf/{scopedRoleMembershipId}
PATCH /scopedRoleMemberships/{scopedRoleMembershipsId}
PATCH /users/{usersId}/scopedRoleMemberOf/{scopedRoleMembershipId}
PATCH /directoryRoles/{directoryRolesId}/scopedMembers/{scopedRoleMembershipId}
PATCH /administrativeUnits/{administrativeUnitsId}/scopedRoleMembers/{scopedRoleMembershipId}
PATCH /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/scopedRoleMembers/{scopedRoleMembershipId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [scopedRoleMembership](../resources/scopedrolemembership.md) object.

The following table shows the properties that are required when you create the [scopedRoleMembership](../resources/scopedrolemembership.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|roleId|String||
|administrativeUnitId|String||
|roleMemberInfo|[identity](../resources/identity.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_scopedrolemembership"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/scopedRoleMemberOf/{scopedRoleMembershipId}
Content-type: application/json
Content-length: 292

{
  "@odata.type": "#microsoft.graph.scopedRoleMembership",
  "roleId": "Role Id value",
  "administrativeUnitId": "Administrative Unit Id value",
  "roleMemberInfo": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value",
    "displayName": "Display Name value"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "@odata.type": "#microsoft.graph.scopedRoleMembership",
  "id": "2c1bda3a-da3a-2c1b-3ada-1b2c3ada1b2c",
  "roleId": "Role Id value",
  "administrativeUnitId": "Administrative Unit Id value",
  "roleMemberInfo": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value",
    "displayName": "Display Name value"
  }
}
```

