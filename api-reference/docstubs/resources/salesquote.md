---
title: "salesQuote resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesQuote resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesQuote](../api/salesquote-get.md)|[salesQuote](../resources/salesquote.md)|Read the properties and relationships of a [salesQuote](../resources/salesquote.md) object.|
|[Update salesQuote](../api/salesquote-update.md)|[salesQuote](../resources/salesquote.md)|Update the properties of a [salesQuote](../resources/salesquote.md) object.|
|[makeInvoice](../api/salesquote-makeinvoice.md)|None|**TODO: Add Description**|
|[send](../api/salesquote-send.md)|None|**TODO: Add Description**|
|[List salesQuoteLines](../api/salesquote-list-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md) collection|Get the salesQuoteLines from the salesQuoteLines navigation property.|
|[Create salesQuoteLines](../api/salesquote-post-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md)|Create a new salesQuoteLines object.|
|[Delete salesQuoteLines](../api/salesquote-delete-salesquotelines.md)|None|Delete a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Update salesQuoteLines](../api/salesquote-update-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md)|Update the properties of a salesQuoteLines object.|
|[Get salesQuoteLine](../api/salesquoteline-get.md)|[salesQuoteLine](../resources/salesquoteline.md)|Read the properties and relationships of a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[List customer](../api/salesquote-list-customer.md)|[customer](../resources/customer.md) collection|Get the customers from the customer navigation property.|
|[Create customer](../api/salesquote-post-customer.md)|[customer](../resources/customer.md)|Create a new customer object.|
|[Delete customer](../api/salesquote-delete-customer.md)|None|Delete a [customer](../resources/customer.md) object.|
|[Update customer](../api/salesquote-update-customer.md)|[customer](../resources/customer.md)|Update the properties of a customer object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read the properties and relationships of a [customer](../resources/customer.md) object.|
|[List currency](../api/salesquote-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/salesquote-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/salesquote-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/salesquote-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/salesquote-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/salesquote-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/salesquote-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/salesquote-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|
|[List shipmentMethod](../api/salesquote-list-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md) collection|Get the shipmentMethods from the shipmentMethod navigation property.|
|[Create shipmentMethod](../api/salesquote-post-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Create a new shipmentMethod object.|
|[Delete shipmentMethod](../api/salesquote-delete-shipmentmethod.md)|None|Delete a [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Update shipmentMethod](../api/salesquote-update-shipmentmethod.md)|[shipmentMethod](../resources/shipmentmethod.md)|Update the properties of a shipmentMethod object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read the properties and relationships of a [shipmentMethod](../resources/shipmentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptedDate|Date|**TODO: Add Description**|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|billToCustomerId|Guid|**TODO: Add Description**|
|billToCustomerNumber|String|**TODO: Add Description**|
|billToName|String|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|documentDate|Date|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|sentDate|DateTimeOffset|**TODO: Add Description**|
|shipmentMethodId|Guid|**TODO: Add Description**|
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shipToContact|String|**TODO: Add Description**|
|shipToName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|validUntilDate|Date|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)|**TODO: Add Description**|
|customer|[customer](../resources/customer.md)|**TODO: Add Description**|
|paymentTerm|[paymentTerm](../resources/paymentterm.md)|**TODO: Add Description**|
|salesQuoteLines|[salesQuoteLine](../resources/salesquoteline.md) collection|**TODO: Add Description**|
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesQuote",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesQuote",
  "id": "String (identifier)",
  "number": "String",
  "externalDocumentNumber": "String",
  "documentDate": "Date",
  "dueDate": "Date",
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
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "String",
  "sentDate": "String (timestamp)",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

