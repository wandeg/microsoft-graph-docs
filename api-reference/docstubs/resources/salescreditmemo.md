---
title: "salesCreditMemo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesCreditMemo resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesCreditMemo](../api/salescreditmemo-get.md)|[salesCreditMemo](../resources/salescreditmemo.md)|Read the properties and relationships of a [salesCreditMemo](../resources/salescreditmemo.md) object.|
|[Update salesCreditMemo](../api/salescreditmemo-update.md)|[salesCreditMemo](../resources/salescreditmemo.md)|Update the properties of a [salesCreditMemo](../resources/salescreditmemo.md) object.|
|[List salesCreditMemoLines](../api/salescreditmemo-list-salescreditmemolines.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md) collection|Get the salesCreditMemoLines from the salesCreditMemoLines navigation property.|
|[Create salesCreditMemoLines](../api/salescreditmemo-post-salescreditmemolines.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md)|Create a new salesCreditMemoLines object.|
|[Delete salesCreditMemoLines](../api/salescreditmemo-delete-salescreditmemolines.md)|None|Delete a [salesCreditMemoLine](../resources/salescreditmemoline.md) object.|
|[Update salesCreditMemoLines](../api/salescreditmemo-update-salescreditmemolines.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md)|Update the properties of a salesCreditMemoLines object.|
|[Get salesCreditMemoLine](../api/salescreditmemoline-get.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md)|Read the properties and relationships of a [salesCreditMemoLine](../resources/salescreditmemoline.md) object.|
|[List customer](../api/salescreditmemo-list-customer.md)|[customer](../resources/customer.md) collection|Get the customers from the customer navigation property.|
|[Create customer](../api/salescreditmemo-post-customer.md)|[customer](../resources/customer.md)|Create a new customer object.|
|[Delete customer](../api/salescreditmemo-delete-customer.md)|None|Delete a [customer](../resources/customer.md) object.|
|[Update customer](../api/salescreditmemo-update-customer.md)|[customer](../resources/customer.md)|Update the properties of a customer object.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read the properties and relationships of a [customer](../resources/customer.md) object.|
|[List currency](../api/salescreditmemo-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/salescreditmemo-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/salescreditmemo-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/salescreditmemo-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List paymentTerm](../api/salescreditmemo-list-paymentterm.md)|[paymentTerm](../resources/paymentterm.md) collection|Get the paymentTerms from the paymentTerm navigation property.|
|[Create paymentTerm](../api/salescreditmemo-post-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Create a new paymentTerm object.|
|[Delete paymentTerm](../api/salescreditmemo-delete-paymentterm.md)|None|Delete a [paymentTerm](../resources/paymentterm.md) object.|
|[Update paymentTerm](../api/salescreditmemo-update-paymentterm.md)|[paymentTerm](../resources/paymentterm.md)|Update the properties of a paymentTerm object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read the properties and relationships of a [paymentTerm](../resources/paymentterm.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|billToCustomerId|Guid|**TODO: Add Description**|
|billToCustomerNumber|String|**TODO: Add Description**|
|billToName|String|**TODO: Add Description**|
|creditMemoDate|Date|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceId|Guid|**TODO: Add Description**|
|invoiceNumber|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
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
|salesCreditMemoLines|[salesCreditMemoLine](../resources/salescreditmemoline.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesCreditMemo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "id": "String (identifier)",
  "number": "String",
  "externalDocumentNumber": "String",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "Guid",
  "customerNumber": "String",
  "customerName": "String",
  "billToName": "String",
  "billToCustomerId": "Guid",
  "billToCustomerNumber": "String",
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
  "currencyId": "Guid",
  "currencyCode": "String",
  "paymentTermsId": "Guid",
  "salesperson": "String",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "invoiceId": "Guid",
  "invoiceNumber": "String",
  "phoneNumber": "String",
  "email": "String"
}
```

