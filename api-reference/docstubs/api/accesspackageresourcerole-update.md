---
title: "Update accessPackageResourceRole"
description: "Update the properties of an accessPackageResourceRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageResourceRole

Namespace: microsoft.graph

Update the properties of an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.

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
PATCH /accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceRole
PATCH /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageResourceRole
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|originId|String|**TODO: Add Description**|
|originSystem|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourcerole"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceRole
Content-Type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value"
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
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "id": "6b4e0f0d-0f0d-6b4e-0d0f-4e6b0d0f4e6b",
  "displayName": "Display Name value",
  "description": "Description value",
  "originId": "Origin Id value",
  "originSystem": "Origin System value"
}
```

