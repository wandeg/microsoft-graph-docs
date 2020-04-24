---
title: "Update printDocument"
description: "Update the properties of a printDocument object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update printDocument

Namespace: microsoft.graph

Update the properties of a [printDocument](../resources/printdocument.md) object.

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
PATCH /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [printDocument](../resources/printdocument.md) object.

The following table shows the properties that are required when you create the [printDocument](../resources/printdocument.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|mimeType|String|**TODO: Add Description**|
|sizeInBytes|Int64|**TODO: Add Description**|
|documentConfiguration|[printerDocumentConfiguration](../resources/printerdocumentconfiguration.md)|**TODO: Add Description**|



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
Content-Type: application/json
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
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "0762466d-466d-0762-6d46-62076d466207",
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

