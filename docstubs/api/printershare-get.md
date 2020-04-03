---
title: "Get printerShare"
description: "Read properties and relationships of the printerShare object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get printerShare

Namespace: microsoft.graph

Read properties and relationships of the [printerShare](../resources/printershare.md) object.

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
GET /print/printerShares/{printerShareId}
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
If successful, this method returns a `200 OK` response code and [printerShare](../resources/printershare.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printerShares/{printerShareId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 214

{
  "value": {
    "@odata.type": "#microsoft.graph.printerShare",
    "id": "a2402444-2444-a240-4424-40a2442440a2",
    "name": "Name value",
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00"
  }
}
```

