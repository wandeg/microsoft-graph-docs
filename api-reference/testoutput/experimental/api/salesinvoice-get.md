---
title: "Get salesInvoice"
description: "Read properties and relationships of the salesInvoice object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesInvoice

Namespace: microsoft.graph

Read properties and relationships of the [salesInvoice](../resources/salesinvoice.md) object.

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
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [salesInvoice](../resources/salesinvoice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesinvoice"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesInvoice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1993

{
  "value": {
    "@odata.type": "#microsoft.graph.salesInvoice",
    "id": "54aaee08-ee08-54aa-08ee-aa5408eeaa54",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "invoiceDate": "Date",
    "dueDate": "Date",
    "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
    "customerId": "7b150b0b-0b0b-7b15-0b0b-157b0b0b157b",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "1bdd7746-7746-1bdd-4677-dd1b4677dd1b",
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
    "currencyId": "3fda09ad-09ad-3fda-ad09-da3fad09da3f",
    "currencyCode": "Currency Code value",
    "orderId": "f7f9d0b6-d0b6-f7f9-b6d0-f9f7b6d0f9f7",
    "orderNumber": "Order Number value",
    "paymentTermsId": "699a59fb-59fb-699a-fb59-9a69fb599a69",
    "shipmentMethodId": "b9539e5d-9e5d-b953-5d9e-53b95d9e53b9",
    "salesperson": "Salesperson value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

