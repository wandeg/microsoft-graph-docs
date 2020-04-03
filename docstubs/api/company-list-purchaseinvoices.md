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
      "id": "91663958-3958-9166-5839-669158396691",
      "number": "Number value",
      "invoiceDate": "Date",
      "dueDate": "Date",
      "vendorInvoiceNumber": "Vendor Invoice Number value",
      "vendorId": "33096b6c-6b6c-3309-6c6b-09336c6b0933",
      "vendorNumber": "Vendor Number value",
      "vendorName": "Vendor Name value",
      "payToName": "Pay To Name value",
      "payToContact": "Pay To Contact value",
      "payToVendorId": "fb77d529-d529-fb77-29d5-77fb29d577fb",
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
      "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
      "currencyCode": "Currency Code value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
    }
  ]
}
```

