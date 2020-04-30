---
title: "Create scopedRoleMembers"
description: "Create a new scopedRoleMembers object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create scopedRoleMembers

Namespace: Microsoft.DirectoryServices

Create a new scopedRoleMembers object.

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
POST /administrativeUnits/{administrativeUnitsId}/scopedRoleMembers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.

The following table shows the properties that are required when you create the [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|administrativeUnitId|String|**TODO: Add Description**|
|roleMemberInfo|[identity](../resources/microsoft.directoryservices-identity.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_scopedrolememberships"
}
-->
``` http
POST https://graph.microsoft.com/changelog/administrativeUnits/{administrativeUnitsId}/scopedRoleMembers
Content-Type: application/json
Content-length: 316

{
  "@odata.type": "#Microsoft.DirectoryServices.scopedRoleMembership",
  "roleId": "Role Id value",
  "administrativeUnitId": "Administrative Unit Id value",
  "roleMemberInfo": {
    "@odata.type": "Microsoft.DirectoryServices.identity",
    "id": "Id value",
    "displayName": "Display Name value"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.scopedrolemembership"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

