---
title: "Create documents"
description: "Create a new documents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create documents

Namespace: microsoft.graph

Create a new documents object.

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
POST /print/printers/{printerId}/jobs/{printJobId}/documents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and a [printDocument](../resources/printdocument.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_printdocument_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{printJobId}/documents
Content-Type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.printDocument",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": "Integer",
  "documentConfiguration": {
    "@odata.type": "microsoft.graph.printerDocumentConfiguration"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printdocument"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```

