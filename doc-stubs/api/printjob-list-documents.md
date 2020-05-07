---
title: "List documents"
description: "Get the printDocuments from the documents navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List documents

Namespace: microsoft.graph

Get the printDocuments from the documents navigation property.

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
GET /print/printers/{printerId}/jobs/{printJobId}/documents
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

If successful, this method returns a `200 OK` response code and a collection of [printDocument](../resources/printdocument.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printdocument"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/documents
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printdocument)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printDocument",
      "id": "49155f82-5f82-4915-825f-1549825f1549",
      "name": "String",
      "mimeType": "String",
      "sizeInBytes": "Integer",
      "documentConfiguration": {
        "@odata.type": "microsoft.graph.printerDocumentConfiguration"
      }
    }
  ]
}
```

