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
    "id": "cb76ebb6-ebb6-cb76-b6eb-76cbb6eb76cb",
    "number": "Number value",
    "invoiceDate": "Date",
    "dueDate": "Date",
    "vendorInvoiceNumber": "Vendor Invoice Number value",
    "vendorId": "003f9ea3-9ea3-003f-a39e-3f00a39e3f00",
    "vendorNumber": "Vendor Number value",
    "vendorName": "Vendor Name value",
    "payToName": "Pay To Name value",
    "payToContact": "Pay To Contact value",
    "payToVendorId": "9ab3cbf6-cbf6-9ab3-f6cb-b39af6cbb39a",
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
    "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
    "currencyCode": "Currency Code value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
  }
}
```

