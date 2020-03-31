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
Content-Length: 1854

{
  "value": {
    "@odata.type": "#microsoft.graph.salesQuote",
    "id": "10d1970c-970c-10d1-0c97-d1100c97d110",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "documentDate": "Date",
    "dueDate": "Date",
    "customerId": "8abcd51d-d51d-8abc-1dd5-bc8a1dd5bc8a",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "fee1cc02-cc02-fee1-02cc-e1fe02cce1fe",
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
    "currencyId": "d358c210-c210-d358-10c2-58d310c258d3",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "2b1121b8-21b8-2b11-b821-112bb821112b",
    "shipmentMethodId": "bc2ec13f-c13f-bc2e-3fc1-2ebc3fc12ebc",
    "salesperson": "Salesperson value",
    "discountAmount": "4.2",
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "sentDate": "2016-12-31T23:57:25.255757+03:00",
    "validUntilDate": "Date",
    "acceptedDate": "Date",
    "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

