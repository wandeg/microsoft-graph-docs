---
title: "Create documents"
description: "Create documents by posting to the documents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create documents

Namespace: microsoft.graph

Create documents by posting to the documents collection.

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
POST /print/printers/{printerId}/jobs/{printJobId}/documents/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printDocument](../resources/printdocument.md) object.

The following table shows the properties that are required when you create the [printDocument](../resources/printdocument.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|mimeType|String||
|sizeInBytes|Int64||
|documentConfiguration|[printerDocumentConfiguration](../resources/printerdocumentconfiguration.md)||



## Response
If successful, this method returns a `201 Created` response code and a [printDocument](../resources/printdocument.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printdocument_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/documents
Content-type: application/json
Content-length: 609

{
  "@odata.type": "#microsoft.graph.printDocument",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printdocument"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 658

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
```

