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
|Name|Description|
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
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices
Content-type: application/json
Content-length: 1769

{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
  "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
  "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
  "currencyCode": "Currency Code value",
  "orderId": "1251b4f2-b4f2-1251-f2b4-5112f2b45112",
  "orderNumber": "Order Number value",
  "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
  "shipmentMethodId": "a8a54da3-4da3-a8a5-a34d-a5a8a34da5a8",
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
  "id": "cf4120d7-20d7-cf41-d720-41cfd72041cf",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
  "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
  "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
  "currencyCode": "Currency Code value",
  "orderId": "1251b4f2-b4f2-1251-f2b4-5112f2b45112",
  "orderNumber": "Order Number value",
  "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
  "shipmentMethodId": "a8a54da3-4da3-a8a5-a34d-a5a8a34da5a8",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

