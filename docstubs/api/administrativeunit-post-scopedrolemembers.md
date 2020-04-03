---
title: "Add scopedRoleMembers"
description: "Add scopedRoleMembers by posting to the scopedRoleMembers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add scopedRoleMembers

Namespace: microsoft.graph

Add scopedRoleMembers by posting to the scopedRoleMembers collection.

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
POST /administrativeUnits/{administrativeUnitsId}/scopedRoleMembers/$ref
POST /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/scopedRoleMembers/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_scopedrolememberships"
}
-->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits/{administrativeUnitsId}/scopedRoleMembers
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
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 341

{
  "@odata.type": "#microsoft.graph.scopedRoleMembership",
  "id": "38485c27-5c27-3848-275c-4838275c4838",
  "roleId": "Role Id value",
  "administrativeUnitId": "Administrative Unit Id value",
  "roleMemberInfo": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value",
    "displayName": "Display Name value"
  }
}
```

