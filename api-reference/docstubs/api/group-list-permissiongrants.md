---
title: "List permissionGrants"
description: "Get the resourceSpecificPermissionGrants from the permissionGrants navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List permissionGrants

Namespace: microsoft.graph

Get the resourceSpecificPermissionGrants from the permissionGrants navigation property.

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
GET ** Collection URI for microsoft.graph.resourceSpecificPermissionGrant not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_resourcespecificpermissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.resourceSpecificPermissionGrant not found
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.resourcespecificpermissiongrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceSpecificPermissionGrant",
      "id": "c5a0e21c-e21c-c5a0-1ce2-a0c51ce2a0c5",
      "deletedDateTime": "String (timestamp)",
      "clientId": "String",
      "clientAppId": "String",
      "resourceAppId": "String",
      "permissionType": "String",
      "permission": "String"
    }
  ]
}
```

