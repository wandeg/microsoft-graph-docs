---
title: "Update salesInvoice"
description: "Update the properties of a salesInvoice object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesInvoice

Namespace: microsoft.graph

Update the properties of a [salesInvoice](../resources/salesinvoice.md) object.

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
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesInvoice](../resources/salesinvoice.md) object.

The following table shows the properties that are required when you create the [salesInvoice](../resources/salesinvoice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|externalDocumentNumber|String||
|invoiceDate|Date||
|dueDate|Date||
|customerPurchaseOrderReference|String||
|customerId|Guid||
|customerNumber|String||
|customerName|String||
|billToName|String||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|shipToName|String||
|shipToContact|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|currencyId|Guid||
|currencyCode|String||
|orderId|Guid||
|orderNumber|String||
|paymentTermsId|Guid||
|shipmentMethodId|Guid||
|salesperson|String||
|pricesIncludeTax|Boolean||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|totalAmountExcludingTax|Decimal||
|totalTaxAmount|Decimal||
|totalAmountIncludingTax|Decimal||
|status|String||
|lastModifiedDateTime|DateTimeOffset||
|phoneNumber|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesInvoice](../resources/salesinvoice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_salesinvoice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
Content-type: application/json
Content-length: 1769

{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "orderId": "92012dfc-2dfc-9201-fc2d-0192fc2d0192",
  "orderNumber": "Order Number value",
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
  "shipmentMethodId": "14ada72c-a72c-14ad-2ca7-ad142ca7ad14",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1882

{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "id": "705f0864-0864-705f-6408-5f7064085f70",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "orderId": "92012dfc-2dfc-9201-fc2d-0192fc2d0192",
  "orderNumber": "Order Number value",
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
  "shipmentMethodId": "14ada72c-a72c-14ad-2ca7-ad142ca7ad14",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

