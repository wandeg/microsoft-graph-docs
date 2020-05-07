---
title: "salesInvoice resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesInvoice resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[cancelAndSend](../api/salesinvoice-cancelandsend.md)|None|**TODO: Add Description**|
|[cancel](../api/salesinvoice-cancel.md)|None|**TODO: Add Description**|
|[postAndSend](../api/salesinvoice-postandsend.md)|None|**TODO: Add Description**|
|[post](../api/salesinvoice-post.md)|None|**TODO: Add Description**|
|[send](../api/salesinvoice-send.md)|None|**TODO: Add Description**|
|[List salesInvoiceLines](../api/salesinvoice-list-salesinvoicelines.md)|[salesInvoiceLine](../resources/salesinvoiceline.md) collection|Get the salesInvoiceLines from the salesInvoiceLines navigation property.|
|[Create salesInvoiceLines](../api/salesinvoice-post-salesinvoicelines.md)|[salesInvoiceLine](../resources/salesinvoiceline.md)|Create a new salesInvoiceLines object.|
|[Delete salesInvoiceLines](../api/salesinvoice-delete-salesinvoicelines.md)|None|Delete a [salesInvoiceLine](../resources/salesinvoiceline.md) object.|
|[Update salesInvoiceLines](../api/salesinvoice-update-salesinvoicelines.md)|[salesInvoiceLine](../resources/salesinvoiceline.md)|Update the properties of a salesInvoiceLines object.|
|[Get salesInvoiceLine](../api/salesinvoiceline-get.md)|[salesInvoiceLine](../resources/salesinvoiceline.md)|Read the properties and relationships of a [salesInvoiceLine](../resources/salesinvoiceline.md) object.|
|[List customer](../api/salesinvoice-list-customer.md)|[customer](../resources/customer.md) collection|Get the customers from the customer navigation property.|
|[Create customer](../api/salesinvoice-post-customer.md)|[customer](../resources/customer.md)|Create a new customer object.|
|[Delete customer](../api/salesinvoice-delete-customer.md)|None|Delete a [customer](../resources/customer.md) object.|
|[Update customer](../api/salesinvoice-update-customer.md)|[customer](../resources/customer.md)|Update the properties of a customer object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read the properties and relationships of a [customer](../resources/customer.md) object.|
|[List currency](../api/salesinvoice-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/salesinvoice-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/salesinvoice-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/salesinvoice-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/salesinvoice-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/salesinvoice-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/salesinvoice-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/salesinvoice-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|
|[List shipmentMethod](../api/salesinvoice-list-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md) collection|Get the shipmentMethods from the shipmentMethod navigation property.|
|[Create shipmentMethod](../api/salesinvoice-post-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Create a new shipmentMethod object.|
|[Delete shipmentMethod](../api/salesinvoice-delete-shipmentmethod.md)|None|Delete a [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Update shipmentMethod](../api/salesinvoice-update-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Update the properties of a shipmentMethod object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read the properties and relationships of a [shipmentMethod](../resources/shipmentmethod.md) object.|
|[List salesInvoices](../api/company-list-salesinvoices.md)|[salesInvoice](../resources/salesinvoice.md) collection|Get the salesInvoices from the salesInvoices navigation property.|
|[Create salesInvoices](../api/company-post-salesinvoices.md)|[salesInvoice](../resources/salesinvoice.md)|Create a new salesInvoices object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|billToCustomerId|Guid|**TODO: Add Description**|
|billToCustomerNumber|String|**TODO: Add Description**|
|billToName|String|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|customerPurchaseOrderReference|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceDate|Date|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|orderId|Guid|**TODO: Add Description**|
|orderNumber|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shipmentMethodId|Guid|**TODO: Add Description**|
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shipToContact|String|**TODO: Add Description**|
|shipToName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)|**TODO: Add Description**|
|customer|[customer](../resources/customer.md)|**TODO: Add Description**|
|paymentTerm|[paymentTerm](../resources/paymentterm.md)|**TODO: Add Description**|
|salesInvoiceLines|[salesInvoiceLine](../resources/salesinvoiceline.md) collection|**TODO: Add Description**|
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesInvoice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "id": "String (identifier)",
  "number": "String",
  "externalDocumentNumber": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "String",
  "customerId": "Guid",
  "customerNumber": "String",
  "customerName": "String",
  "billToName": "String",
  "billToCustomerId": "Guid",
  "billToCustomerNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "sellingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "billingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shippingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "orderId": "Guid",
  "orderNumber": "String",
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

