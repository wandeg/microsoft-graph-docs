---
title: "Get currency"
description: "Read properties and relationships of the currency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get currency

Read properties and relationships of the [currency](../resources/currency.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/currencies/{currencyId}
GET /financials/companies/{companyId}/vendors/{vendorId}/currency
GET /financials/companies/{companyId}/customers/{customerId}/currency
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/currency
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/currency
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/currency
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/currency
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/currency
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [currency](../resources/currency.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_currency"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/currencies/{currencyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.currency"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 386

{
  "value": {
    "@odata.type": "#microsoft.graph.currency",
    "id": "d7d2ba6d-ba6d-d7d2-6dba-d2d76dbad2d7",
    "code": "Code value",
    "displayName": "Display Name value",
    "symbol": "Symbol value",
    "amountDecimalPlaces": "Amount Decimal Places value",
    "amountRoundingPrecision": "4.2",
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
  }
}
```

