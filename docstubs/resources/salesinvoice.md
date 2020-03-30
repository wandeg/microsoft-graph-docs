---
title: "salesInvoice resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# salesInvoice resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesInvoice](../api/salesinvoice-get.md)|[salesInvoice](../resources/salesinvoice.md)|Read properties and relationships of the [salesInvoice](../resources/salesinvoice.md) object.|
|[Update salesInvoice](../api/salesinvoice-update.md)|[salesInvoice](../resources/salesinvoice.md)|Update the properties of a [salesInvoice](../resources/salesinvoice.md) object.|
|[cancelAndSend](../api/salesinvoice-cancelandsend.md)|None||
|[cancel](../api/salesinvoice-cancel.md)|None||
|[postAndSend](../api/salesinvoice-postandsend.md)|None||
|[post](../api/salesinvoice-post.md)|None||
|[send](../api/salesinvoice-send.md)|None||
|[List salesInvoiceLines](../api/salesinvoice-list-salesinvoicelines.md)|[salesInvoiceLine](../resources/salesinvoiceline.md) collection|Get the salesInvoiceLines from the salesInvoiceLines navigation property.|
|[Add salesInvoiceLines](../api/salesinvoice-post-salesinvoicelines.md)|[salesInvoiceLine](../resources/salesinvoiceline.md)|Add salesInvoiceLines by posting to the salesInvoiceLines collection.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|billToName|String||
|currencyCode|String||
|currencyId|Guid||
|customerId|Guid||
|customerName|String||
|customerNumber|String||
|customerPurchaseOrderReference|String||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|dueDate|Date||
|email|String||
|externalDocumentNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceDate|Date||
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|orderId|Guid||
|orderNumber|String||
|paymentTermsId|Guid||
|phoneNumber|String||
|pricesIncludeTax|Boolean||
|salesperson|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shipmentMethodId|Guid||
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shipToContact|String||
|shipToName|String||
|status|String||
|totalAmountExcludingTax|Decimal||
|totalAmountIncludingTax|Decimal||
|totalTaxAmount|Decimal||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)||
|customer|[customer](../resources/customer.md)||
|paymentTerm|[paymentTerm](../resources/paymentterm.md)||
|salesInvoiceLines|[salesInvoiceLine](../resources/salesinvoiceline.md) collection||
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)||

## JSON representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryLetterCode": "String",
    "postalCode": "String"
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
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

