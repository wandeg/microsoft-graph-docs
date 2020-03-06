---
title: "Update purchaseInvoice"
description: "Update the properties of a purchaseInvoice object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update purchaseInvoice

Namespace: microsoft.graph

Update the properties of a [purchaseInvoice](../resources/purchaseinvoice.md) object.

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
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [purchaseInvoice](../resources/purchaseinvoice.md) object.

The following table shows the properties that are required when you create the [purchaseInvoice](../resources/purchaseinvoice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|invoiceDate|Date||
|dueDate|Date||
|vendorInvoiceNumber|String||
|vendorId|Guid||
|vendorNumber|String||
|vendorName|String||
|payToName|String||
|payToContact|String||
|payToVendorId|Guid||
|payToVendorNumber|String||
|shipToName|String||
|shipToContact|String||
|buyFromAddress|[postalAddressType](../resources/postaladdresstype.md)||
|payToAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shipToAddress|[postalAddressType](../resources/postaladdresstype.md)||
|currencyId|Guid||
|currencyCode|String||
|pricesIncludeTax|Boolean||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|totalAmountExcludingTax|Decimal||
|totalTaxAmount|Decimal||
|totalAmountIncludingTax|Decimal||
|status|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [purchaseInvoice](../resources/purchaseinvoice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_purchaseinvoice"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
Content-type: application/json
Content-length: 1362

{
  "@odata.type": "#microsoft.graph.purchaseInvoice",
  "number": "Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "vendorInvoiceNumber": "Vendor Invoice Number value",
  "vendorId": "518a2703-2703-518a-0327-8a5103278a51",
  "vendorNumber": "Vendor Number value",
  "vendorName": "Vendor Name value",
  "payToName": "Pay To Name value",
  "payToContact": "Pay To Contact value",
  "payToVendorId": "fa69a03d-a03d-fa69-3da0-69fa3da069fa",
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
  "currencyId": "3fda09ad-09ad-3fda-ad09-da3fad09da3f",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1475

{
  "@odata.type": "#microsoft.graph.purchaseInvoice",
  "id": "cb0c180a-180a-cb0c-0a18-0ccb0a180ccb",
  "number": "Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "vendorInvoiceNumber": "Vendor Invoice Number value",
  "vendorId": "518a2703-2703-518a-0327-8a5103278a51",
  "vendorNumber": "Vendor Number value",
  "vendorName": "Vendor Name value",
  "payToName": "Pay To Name value",
  "payToContact": "Pay To Contact value",
  "payToVendorId": "fa69a03d-a03d-fa69-3da0-69fa3da069fa",
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
  "currencyId": "3fda09ad-09ad-3fda-ad09-da3fad09da3f",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
}
```

