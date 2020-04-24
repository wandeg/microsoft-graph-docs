---
title: "List schemaExtensions"
description: "Get a list of the schemaExtension objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List schemaExtensions

Namespace: microsoft.graph

Get a list of the [schemaExtension](../resources/schemaextension.md) objects and their properties.

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
GET /schemaExtensions
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
If successful, this method returns a `200 OK` response code and a collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}
-->
``` http
GET https://graph.microsoft.com/beta/schemaExtensions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.schemaextension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.schemaExtension",
      "id": "7a4131b7-31b7-7a41-b731-417ab731417a",
      "description": "Description value",
      "targetTypes": [
        "Target Types value"
      ],
      "properties": [
        {
          "@odata.type": "microsoft.graph.extensionSchemaProperty",
          "name": "Name value",
          "type": "Type value"
        }
      ],
      "status": "Status value",
      "owner": "Owner value"
    }
  ]
}
```

