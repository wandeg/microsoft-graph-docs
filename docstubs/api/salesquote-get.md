---
title: "Get salesQuote"
description: "Read properties and relationships of the salesQuote object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesQuote

Namespace: microsoft.graph

Read properties and relationships of the [salesQuote](../resources/salesquote.md) object.

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
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}
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
If successful, this method returns a `200 OK` response code and [salesQuote](../resources/salesquote.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesquote"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesQuote"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1856

{
  "value": {
    "@odata.type": "#microsoft.graph.salesQuote",
    "id": "c488d060-d060-c488-60d0-88c460d088c4",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "documentDate": "Date",
    "dueDate": "Date",
    "customerId": "96a89bff-9bff-96a8-ff9b-a896ff9ba896",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "9b1f7785-7785-9b1f-8577-1f9b85771f9b",
    "billToCustomerNumber": "Bill To Customer Number value",
    "shipToName": "Ship To Name value",
    "shipToContact": "Ship To Contact value",
    "sellingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryLetterCode": "Country Letter Code value",
      "postalCode": "Postal Code value"
    },
    "billingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "shippingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "currencyId": "93b64d88-4d88-93b6-884d-b693884db693",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "8173a089-a089-8173-89a0-738189a07381",
    "shipmentMethodId": "85041d67-1d67-8504-671d-0485671d0485",
    "salesperson": "Salesperson value",
    "discountAmount": "4.2",
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "sentDate": "2016-12-31T23:57:13.8772583+03:00",
    "validUntilDate": "Date",
    "acceptedDate": "Date",
    "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

