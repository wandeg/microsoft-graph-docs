---
title: "Update accessPackageResourceRoleScopes"
description: "Update the properties of an accessPackageResourceRoleScopes object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessPackageResourceRoleScopes

Namespace: microsoft.graph

Update the properties of an accessPackageResourceRoleScopes object.

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
PATCH ** Collection URI for microsoft.graph.accessPackageResourceRoleScope not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accesspackageresourcerolescopes"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.graph.accessPackageResourceRoleScope not found
Content-Type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "createdBy": "String",
  "modifiedBy": "String"
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
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "680f67c4-67c4-680f-c467-0f68c4670f68",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

