---
title: "Update printDocument"
description: "Update the properties of a printDocument object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printDocument

Namespace: microsoft.graph

Update the properties of a [printDocument](../resources/printdocument.md) object.

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
PATCH /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [printDocument](../resources/printdocument.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printdocument"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 658

{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "2191d268-d268-2191-68d2-912168d29121",
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

