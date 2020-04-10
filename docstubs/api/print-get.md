---
title: "Get print"
description: "Read properties and relationships of the print object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get print

Namespace: microsoft.graph

Read properties and relationships of the [print](../resources/print.md) object.

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
GET /print
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
If successful, this method returns a `200 OK` response code and [print](../resources/print.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_print"
}
-->
``` http
GET https://graph.microsoft.com/beta/print
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.print"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.print",
    "id": "aa8b615f-615f-aa8b-5f61-8baa5f618baa",
    "settings": {
      "@odata.type": "microsoft.graph.printSettings",
      "documentConversionEnabled": true
    }
  }
}
```

