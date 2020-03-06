---
title: "Add salesInvoices"
description: "Add salesInvoices by posting to the salesInvoices collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesInvoices

Namespace: microsoft.graph

Add salesInvoices by posting to the salesInvoices collection.

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
POST /financials/companies/{companyId}/salesInvoices/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [salesInvoice](../resources/salesinvoice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salesinvoice_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesInvoices
Content-type: application/json
Content-length: 1769

{
  "@odata.type": "#microsoft.graph.salesInvoice",
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
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesinvoice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1882

{
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
```

