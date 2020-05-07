---
title: "Get currency"
description: "Read the properties and relationships of a currency object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get currency

Namespace: microsoft.graph

Read the properties and relationships of a [currency](../resources/currency.md) object.

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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [currency](../resources/currency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_currency"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/currencies/{currencyId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.currency"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.currency",
    "id": "edbd813b-813b-edbd-3b81-bded3b81bded",
    "code": "String",
    "displayName": "String",
    "symbol": "String",
    "amountDecimalPlaces": "String",
    "amountRoundingPrecision": "Decimal",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

