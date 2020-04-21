---
title: "Get schemaExtension"
description: "Read properties and relationships of a schemaExtension object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get schemaExtension

Namespace: microsoft.graph

Read properties and relationships of a [schemaExtension](../resources/schemaextension.md) object.

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
GET /schemaExtensions/{schemaExtensionsId}
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
If successful, this method returns a `200 OK` response code and a [schemaExtension](../resources/schemaextension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}
-->
``` http
GET https://graph.microsoft.com/beta/schemaExtensions/{schemaExtensionsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.schemaExtension",
    "id": "da395e08-5e08-da39-085e-39da085e39da",
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
}
```

