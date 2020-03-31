---
title: "List taxAreas"
description: "Get the taxAreas from the taxAreas navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List taxAreas

Namespace: microsoft.graph

Get the taxAreas from the taxAreas navigation property.

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
GET /financials/companies/{companyId}/taxAreas
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
If successful, this method returns a `200 OK` response code and a collection of [taxArea](../resources/taxarea.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_taxarea"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/taxAreas
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.taxarea)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.taxArea",
      "id": "902e4554-4554-902e-5445-2e9054452e90",
      "code": "Code value",
      "displayName": "Display Name value",
      "taxType": "Tax Type value",
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
    }
  ]
}
```

