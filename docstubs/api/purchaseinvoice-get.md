---
title: "Get purchaseInvoice"
description: "Read properties and relationships of the purchaseInvoice object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get purchaseInvoice

Namespace: microsoft.graph

Read properties and relationships of the [purchaseInvoice](../resources/purchaseinvoice.md) object.

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
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
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
If successful, this method returns a `200 OK` response code and [purchaseInvoice](../resources/purchaseinvoice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoice"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.purchaseInvoice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1572

{
  "value": {
    "@odata.type": "#microsoft.graph.purchaseInvoice",
    "id": "6b325954-5954-6b32-5459-326b5459326b",
    "number": "Number value",
    "invoiceDate": "Date",
    "dueDate": "Date",
    "vendorInvoiceNumber": "Vendor Invoice Number value",
    "vendorId": "2ab48266-8266-2ab4-6682-b42a6682b42a",
    "vendorNumber": "Vendor Number value",
    "vendorName": "Vendor Name value",
    "payToName": "Pay To Name value",
    "payToContact": "Pay To Contact value",
    "payToVendorId": "8b11da5e-da5e-8b11-5eda-118b5eda118b",
    "payToVendorNumber": "Pay To Vendor Number value",
    "shipToName": "Ship To Name value",
    "shipToContact": "Ship To Contact value",
    "buyFromAddress": {
      "@odata.type": "microsoft.graph.postalAddressType",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryLetterCode": "Country Letter Code value",
      "postalCode": "Postal Code value"
    },
    "payToAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "shipToAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "currencyId": "5718300d-300d-5718-0d30-18570d301857",
    "currencyCode": "Currency Code value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
  }
}
```

