---
title: "List documents"
description: "Get the printDocuments from the documents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List documents

Namespace: microsoft.graph

Get the printDocuments from the documents navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [printDocument](../resources/printdocument.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printdocument"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/documents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printdocument)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printDocument",
      "id": "e5ea3089-3089-e5ea-8930-eae58930eae5",
      "name": "Name value",
      "mimeType": "Mime Type value",
      "sizeInBytes": 11,
      "documentConfiguration": {
        "@odata.type": "microsoft.graph.printerDocumentConfiguration",
        "pageRanges": [
          {
            "@odata.type": "microsoft.graph.printPageRange",
            "startPage": 9,
            "endPage": 7
          }
        ],
        "printQuality": "String",
        "printResolutionInDpi": 4,
        "feedDirection": "String",
        "orientation": "String",
        "duplexConfiguration": "String",
        "copies": 6,
        "colorConfiguration": "String"
      }
    }
  ]
}
```

