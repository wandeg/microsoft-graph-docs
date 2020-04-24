---
title: "Update scopedRoleMemberOf"
description: "Update the properties of a scopedRoleMemberOf object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update scopedRoleMemberOf

Namespace: microsoft.graph

Update the properties of a scopedRoleMemberOf object.

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
PATCH /me/scopedRoleMemberOf
PATCH /users/{usersId}/scopedRoleMemberOf
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [scopedRoleMembership](../resources/scopedrolemembership.md) object.

The following table shows the properties that are required when you create the [scopedRoleMembership](../resources/scopedrolemembership.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roleId|String|**TODO: Add Description**|
|administrativeUnitId|String|**TODO: Add Description**|
|roleMemberInfo|[identity](../resources/identity.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_scopedrolememberof"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/scopedRoleMemberOf
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.scopedRoleMembership",
  "id": "47b938e2-38e2-47b9-e238-b947e238b947",
  "roleId": "Role Id value",
  "administrativeUnitId": "Administrative Unit Id value",
  "roleMemberInfo": {
    "@odata.type": "microsoft.graph.identity",
    "id": "Id value",
    "displayName": "Display Name value"
  }
}
```

