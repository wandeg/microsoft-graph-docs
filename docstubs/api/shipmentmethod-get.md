---
title: "Get shipmentMethod"
description: "Read properties and relationships of the shipmentMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get shipmentMethod

Namespace: microsoft.graph

Read properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) object.

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
GET /financials/companies/{companyId}/shipmentMethods/{shipmentMethodId}
GET /financials/companies/{companyId}/customers/{customerId}/shipmentMethod
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/shipmentMethod
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/shipmentMethod
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
If successful, this method returns a `200 OK` response code and [shipmentMethod](../resources/shipmentmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shipmentmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/shipmentMethods/{shipmentMethodId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shipmentMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.shipmentMethod",
    "id": "bf38698a-698a-bf38-8a69-38bf8a6938bf",
    "code": "Code value",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00"
  }
}
```

