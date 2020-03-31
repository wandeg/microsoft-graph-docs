---
title: "List purchaseInvoices"
description: "Get the purchaseInvoices from the purchaseInvoices navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List purchaseInvoices

Namespace: microsoft.graph

Get the purchaseInvoices from the purchaseInvoices navigation property.

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
GET /financials/companies/{companyId}/purchaseInvoices
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
If successful, this method returns a `200 OK` response code and a collection of [purchaseInvoice](../resources/purchaseinvoice.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoice"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoices
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
      "id": "c3717303-7303-c371-0373-71c3037371c3",
      "number": "Number value",
      "invoiceDate": "Date",
      "dueDate": "Date",
      "vendorInvoiceNumber": "Vendor Invoice Number value",
      "vendorId": "7d860597-0597-7d86-9705-867d9705867d",
      "vendorNumber": "Vendor Number value",
      "vendorName": "Vendor Name value",
      "payToName": "Pay To Name value",
      "payToContact": "Pay To Contact value",
      "payToVendorId": "8bee7144-7144-8bee-4471-ee8b4471ee8b",
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
      "currencyId": "cf2f699a-699a-cf2f-9a69-2fcf9a692fcf",
      "currencyCode": "Currency Code value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00"
    }
  ]
}
```

