---
title: "salesOrder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# salesOrder resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesOrder](../api/salesorder-get.md)|[salesOrder](../resources/salesOrder.md)|Read properties and relationships of the [salesOrder](../resources/salesorder.md) object.|
|[Delete salesOrder](../api/salesorder-delete.md)|None|Deletes a [salesOrder](../resources/salesorder.md).|
|[Update salesOrder](../api/salesorder-update.md)|[salesOrder](../resources/salesOrder.md)|Update the properties of a [salesOrder](../resources/salesorder.md) object.|
|[List salesOrderLines](../api/salesorder-list-salesorderlines.md)|[salesOrderLine](../resources/salesOrderLine.md) collection|Get the salesOrderLines from the salesOrderLines navigation property.|
|[Add salesOrderLines](../api/salesorder-post-salesorderlines.md)|[salesOrderLine](../resources/salesOrderLine.md)|Add salesOrderLines by posting to the salesOrderLines collection.|
|[Get customer](../api/customer-get.md)|[customer](../resources/customer.md)|Read properties and relationships of the [customer](../resources/customer.md) object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentTerm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|billingPostalAddress|[postalAddressType](../resources/postalAddressType.md)||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|billToName|String||
|currencyCode|String||
|currencyId|Guid||
|customerId|Guid||
|customerName|String||
|customerNumber|String||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|email|String||
|externalDocumentNumber|String||
|fullyShipped|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|orderDate|Date||
|partialShipping|Boolean||
|paymentTermsId|Guid||
|phoneNumber|String||
|pricesIncludeTax|Boolean||
|requestedDeliveryDate|Date||
|salesperson|String||
|sellingPostalAddress|[postalAddressType](../resources/postalAddressType.md)||
|shippingPostalAddress|[postalAddressType](../resources/postalAddressType.md)||
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
|paymentTerm|[paymentTerm](../resources/paymentTerm.md)||
|salesOrderLines|[salesOrderLine](../resources/salesOrderLine.md) collection||

## JSON Representation
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

