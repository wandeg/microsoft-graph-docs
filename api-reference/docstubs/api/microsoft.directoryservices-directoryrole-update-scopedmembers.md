---
title: "Update scopedMembers"
description: "Update the properties of a scopedMembers object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update scopedMembers

Namespace: Microsoft.DirectoryServices

Update the properties of a scopedMembers object.

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
PATCH /directoryRoles/{directoryRolesId}/scopedMembers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_scopedmembers"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/directoryRoles/{directoryRolesId}/scopedMembers
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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

