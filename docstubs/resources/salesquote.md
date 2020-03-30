---
title: "salesQuote resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# salesQuote resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesQuote](../api/salesquote-get.md)|[salesQuote](../resources/salesquote.md)|Read properties and relationships of the [salesQuote](../resources/salesquote.md) object.|
|[Update salesQuote](../api/salesquote-update.md)|[salesQuote](../resources/salesquote.md)|Update the properties of a [salesQuote](../resources/salesquote.md) object.|
|[makeInvoice](../api/salesquote-makeinvoice.md)|None||
|[send](../api/salesquote-send.md)|None||
|[List salesQuoteLines](../api/salesquote-list-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md) collection|Get the salesQuoteLines from the salesQuoteLines navigation property.|
|[Add salesQuoteLines](../api/salesquote-post-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md)|Add salesQuoteLines by posting to the salesQuoteLines collection.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptedDate|Date||
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|billToName|String||
|currencyCode|String||
|currencyId|Guid||
|customerId|Guid||
|customerName|String||
|customerNumber|String||
|discountAmount|Decimal||
|documentDate|Date||
|dueDate|Date||
|email|String||
|externalDocumentNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|paymentTermsId|Guid||
|phoneNumber|String||
|salesperson|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|sentDate|DateTimeOffset||
|shipmentMethodId|Guid||
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shipToContact|String||
|shipToName|String||
|status|String||
|totalAmountExcludingTax|Decimal||
|totalAmountIncludingTax|Decimal||
|totalTaxAmount|Decimal||
|validUntilDate|Date||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)||
|customer|[customer](../resources/customer.md)||
|paymentTerm|[paymentTerm](../resources/paymentterm.md)||
|salesQuoteLines|[salesQuoteLine](../resources/salesquoteline.md) collection||
|shipmentMethod|[shipmentMethod](../resources/shipmentmethod.md)||

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

