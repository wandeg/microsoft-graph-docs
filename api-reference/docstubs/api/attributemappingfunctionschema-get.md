---
title: "Get attributeMappingFunctionSchema"
description: "Read the properties and relationships of an attributeMappingFunctionSchema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get attributeMappingFunctionSchema

Namespace: microsoft.graph

Read the properties and relationships of an [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.

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
GET /functions/{functionsId}
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
If successful, this method returns a `200 OK` response code and an [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_attributemappingfunctionschema"
}
-->
``` http
GET https://graph.microsoft.com/beta/functions/{functionsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
    "id": "460e56ef-56ef-460e-ef56-0e46ef560e46",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.attributeMappingParameterSchema",
        "allowMultipleOccurrences": true,
        "name": "Name value",
        "required": true,
        "type": "String"
      }
    ]
  }
}
```

