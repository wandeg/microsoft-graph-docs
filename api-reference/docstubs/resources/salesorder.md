---
title: "salesOrder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesOrder resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesOrder](../api/salesorder-get.md)|[salesOrder](../resources/salesorder.md)|Read the properties and relationships of a [salesOrder](../resources/salesorder.md) object.|
|[Update salesOrder](../api/salesorder-update.md)|[salesOrder](../resources/salesorder.md)|Update the properties of a [salesOrder](../resources/salesorder.md) object.|
|[List salesOrderLines](../api/salesorder-list-salesorderlines.md)|[salesOrderLine](../resources/salesorderline.md) collection|Get the salesOrderLines from the salesOrderLines navigation property.|
|[Create salesOrderLines](../api/salesorder-post-salesorderlines.md)|[salesOrderLine](../resources/salesorderline.md)|Create a new salesOrderLines object.|
|[Delete salesOrderLines](../api/salesorder-delete-salesorderlines.md)|None|Delete a [salesOrderLine](../resources/salesorderline.md) object.|
|[Update salesOrderLines](../api/salesorder-update-salesorderlines.md)|[salesOrderLine](../resources/salesorderline.md)|Update the properties of a salesOrderLines object.|
|[Get salesOrderLine](../api/salesorderline-get.md)|[salesOrderLine](../resources/salesorderline.md)|Read the properties and relationships of a [salesOrderLine](../resources/salesorderline.md) object.|
|[List customer](../api/salesorder-list-customer.md)|[customer](../resources/customer.md) collection|Get the customers from the customer navigation property.|
|[Create customer](../api/salesorder-post-customer.md)|[customer](../resources/customer.md)|Create a new customer object.|
|[Delete customer](../api/salesorder-delete-customer.md)|None|Delete a [customer](../resources/customer.md) object.|
|[Update customer](../api/salesorder-update-customer.md)|[customer](../resources/customer.md)|Update the properties of a customer object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read the properties and relationships of a [customer](../resources/customer.md) object.|
|[List currency](../api/salesorder-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/salesorder-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/salesorder-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/salesorder-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/salesorder-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/salesorder-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/salesorder-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/salesorder-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|

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
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|fullyShipped|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|orderDate|Date|**TODO: Add Description**|
|partialShipping|Boolean|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|requestedDeliveryDate|Date|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
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
|salesOrderLines|[salesOrderLine](../resources/salesorderline.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesOrder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesOrder",
  "id": "String (identifier)",
  "number": "String",
  "externalDocumentNumber": "String",
  "orderDate": "Date",
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
  "pricesIncludeTax": true,
  "paymentTermsId": "Guid",
  "salesperson": "String",
  "partialShipping": true,
  "requestedDeliveryDate": "Date",
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "fullyShipped": true,
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

