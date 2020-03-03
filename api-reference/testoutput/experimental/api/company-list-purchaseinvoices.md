---
title: "List purchaseInvoices"
description: "Get the purchaseInvoices from the purchaseInvoices navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List purchaseInvoices

Get the purchaseInvoices from the purchaseInvoices navigation property.

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
GET /financials/companies/{companyId}/purchaseInvoices
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [purchaseInvoice](../resources/purchaseinvoice.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoice"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/purchaseInvoices
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.purchaseinvoice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.purchaseInvoice",
      "id": "6afd685a-685a-6afd-5a68-fd6a5a68fd6a",
      "number": "Number value",
      "invoiceDate": "Date",
      "dueDate": "Date",
      "vendorInvoiceNumber": "Vendor Invoice Number value",
      "vendorId": "1e46ebdc-ebdc-1e46-dceb-461edceb461e",
      "vendorNumber": "Vendor Number value",
      "vendorName": "Vendor Name value",
      "payToName": "Pay To Name value",
      "payToContact": "Pay To Contact value",
      "payToVendorId": "6e6d7366-7366-6e6d-6673-6d6e66736d6e",
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
      "currencyId": "20bf8064-8064-20bf-6480-bf206480bf20",
      "currencyCode": "Currency Code value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
    }
  ]
}
```

