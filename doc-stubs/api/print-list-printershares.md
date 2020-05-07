---
title: "List printerShares"
description: "Get the printerShares from the printerShares navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List printerShares

Namespace: microsoft.graph

Get the printerShares from the printerShares navigation property.

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
GET /print/printerShares
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

If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printerShares
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printershare)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printerShare",
      "id": "1c31be74-be74-1c31-74be-311c74be311c",
      "name": "String",
      "manufacturer": "String",
      "model": "String",
      "isAcceptingJobs": "Boolean",
      "defaults": {
        "@odata.type": "microsoft.graph.printerDefaults"
      },
      "location": {
        "@odata.type": "microsoft.graph.printerLocation"
      },
      "capabilities": {
        "@odata.type": "microsoft.graph.printerCapabilities"
      },
      "status": {
        "@odata.type": "microsoft.graph.printerStatus"
      },
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```

