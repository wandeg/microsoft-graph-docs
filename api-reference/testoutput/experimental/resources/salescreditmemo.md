---
title: "salesCreditMemo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# salesCreditMemo resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesCreditMemo](../api/salescreditmemo-get.md)|[salesCreditMemo](../resources/salescreditmemo.md)|Read properties and relationships of the [salesCreditMemo](../resources/salescreditmemo.md) object.|
|[Update salesCreditMemo](../api/salescreditmemo-update.md)|[salesCreditMemo](../resources/salescreditmemo.md)|Update the properties of a [salesCreditMemo](../resources/salescreditmemo.md) object.|
|[List salesCreditMemoLines](../api/salescreditmemo-list-salescreditmemolines.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md) collection|Get the salesCreditMemoLines from the salesCreditMemoLines navigation property.|
|[Add salesCreditMemoLines](../api/salescreditmemo-post-salescreditmemolines.md)|[salesCreditMemoLine](../resources/salescreditmemoline.md)|Add salesCreditMemoLines by posting to the salesCreditMemoLines collection.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentterm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[List salesCreditMemos](../api/company-list-salescreditmemos.md)|[salesCreditMemo](../resources/salescreditmemo.md) collection|Get the salesCreditMemos from the salesCreditMemos navigation property.|
|[Add salesCreditMemos](../api/company-post-salescreditmemos.md)|[salesCreditMemo](../resources/salescreditmemo.md)|Add salesCreditMemos by posting to the salesCreditMemos collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|billToName|String||
|creditMemoDate|Date||
|currencyCode|String||
|currencyId|Guid||
|customerId|Guid||
|customerName|String||
|customerNumber|String||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|dueDate|Date||
|email|String||
|externalDocumentNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceId|Guid||
|invoiceNumber|String||
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|paymentTermsId|Guid||
|phoneNumber|String||
|pricesIncludeTax|Boolean||
|salesperson|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
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
|salesCreditMemoLines|[salesCreditMemoLine](../resources/salescreditmemoline.md) collection||

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

