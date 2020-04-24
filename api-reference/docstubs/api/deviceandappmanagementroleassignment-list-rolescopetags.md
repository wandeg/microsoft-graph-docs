---
title: "List roleScopeTags"
description: "Get the roleScopeTags from the roleScopeTags navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List roleScopeTags

Namespace: microsoft.graph

Get the roleScopeTags from the roleScopeTags navigation property.

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
GET ** Collection URI for microsoft.graph.roleScopeTag not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/rolescopetag.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_rolescopetag"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.roleScopeTag not found
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.rolescopetag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "6e4aa040-a040-6e4a-40a0-4a6e40a04a6e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```

