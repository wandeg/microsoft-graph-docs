---
title: "List salesInvoices"
description: "List properties and relationships of the salesInvoice objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesInvoices

Namespace: microsoft.graph

List properties and relationships of the [salesInvoice](../resources/salesinvoice.md) objects.

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
GET /financials/companies/{companyId}/salesInvoices
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [salesInvoice](../resources/salesinvoice.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesinvoice"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesInvoices
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesinvoice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2099

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesInvoice",
      "id": "d96040c5-40c5-d960-c540-60d9c54060d9",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "invoiceDate": "Date",
      "dueDate": "Date",
      "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
      "customerId": "a61f8986-8986-a61f-8689-1fa686891fa6",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "7a1538dc-38dc-7a15-dc38-157adc38157a",
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
      "currencyId": "5323df69-df69-5323-69df-235369df2353",
      "currencyCode": "Currency Code value",
      "orderId": "ebd7b55b-b55b-ebd7-5bb5-d7eb5bb5d7eb",
      "orderNumber": "Order Number value",
      "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
      "shipmentMethodId": "29227862-7862-2922-6278-222962782229",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

