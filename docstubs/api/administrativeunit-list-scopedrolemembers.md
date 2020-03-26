---
title: "List scopedRoleMembers"
description: "Get the scopedRoleMemberships from the scopedRoleMembers navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List scopedRoleMembers

Namespace: microsoft.graph

Get the scopedRoleMemberships from the scopedRoleMembers navigation property.

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
GET /administrativeUnits/{administrativeUnitsId}/scopedRoleMembers
GET /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/scopedRoleMembers
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
If successful, this method returns a `200 OK` response code and a collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemembership"
}
-->
``` http
GET https://graph.microsoft.com/beta/administrativeUnits/{administrativeUnitsId}/scopedRoleMembers
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.scopedrolemembership)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.scopedRoleMembership",
      "id": "04baf8bb-f8bb-04ba-bbf8-ba04bbf8ba04",
      "roleId": "Role Id value",
      "administrativeUnitId": "Administrative Unit Id value",
      "roleMemberInfo": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    }
  ]
}
```

