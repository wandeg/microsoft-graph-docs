---
title: "Create accessPackageResourceRole"
description: "Create a new accessPackageResourceRole object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageResourceRole

Namespace: microsoft.graph

Create a new accessPackageResourceRole object.

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
POST /accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceRole
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerole_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageResourceRoleScopes/{accessPackageResourceRoleScopesId}/accessPackageResourceRole
Content-Type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "id": "745f5a11-5a11-745f-115a-5f74115a5f74",
  "displayName": "String",
  "description": "String",
  "originId": "String",
  "originSystem": "String"
}
```

