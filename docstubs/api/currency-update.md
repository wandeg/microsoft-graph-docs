---
title: "Update currency"
description: "Update the properties of a currency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update currency

Namespace: microsoft.graph

Update the properties of a [currency](../resources/currency.md) object.

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
PATCH /financials/companies/{companyId}/currencies/{currencyId}
PATCH /financials/companies/{companyId}/vendors/{vendorId}/currency
PATCH /financials/companies/{companyId}/customers/{customerId}/currency
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/currency
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/currency
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/currency
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/currency
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/currency
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [currency](../resources/currency.md) object.

The following table shows the properties that are required when you create the [currency](../resources/currency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|symbol|String||
|amountDecimalPlaces|String||
|amountRoundingPrecision|Decimal||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [currency](../resources/currency.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_currency"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/currencies/{currencyId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.currency",
  "code": "Code value",
  "displayName": "Display Name value",
  "symbol": "Symbol value",
  "amountDecimalPlaces": "Amount Decimal Places value",
  "amountRoundingPrecision": "4.2"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.currency",
  "id": "716ded7b-ed7b-716d-7bed-6d717bed6d71",
  "code": "Code value",
  "displayName": "Display Name value",
  "symbol": "Symbol value",
  "amountDecimalPlaces": "Amount Decimal Places value",
  "amountRoundingPrecision": "4.2",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

