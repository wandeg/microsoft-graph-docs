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
      "id": "918d4830-4830-918d-3048-8d9130488d91",
      "number": "Number value",
      "invoiceDate": "Date",
      "dueDate": "Date",
      "vendorInvoiceNumber": "Vendor Invoice Number value",
      "vendorId": "ccf801f6-01f6-ccf8-f601-f8ccf601f8cc",
      "vendorNumber": "Vendor Number value",
      "vendorName": "Vendor Name value",
      "payToName": "Pay To Name value",
      "payToContact": "Pay To Contact value",
      "payToVendorId": "33281f1c-1f1c-3328-1c1f-28331c1f2833",
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
      "currencyId": "93b64d88-4d88-93b6-884d-b693884db693",
      "currencyCode": "Currency Code value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00"
    }
  ]
}
```

