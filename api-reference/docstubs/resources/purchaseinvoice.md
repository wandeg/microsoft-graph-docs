---
title: "purchaseInvoice resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# purchaseInvoice resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get purchaseInvoice](../api/purchaseinvoice-get.md)|[purchaseInvoice](../resources/purchaseinvoice.md)|Read properties and relationships of the [purchaseInvoice](../resources/purchaseinvoice.md) object.|
|[Update purchaseInvoice](../api/purchaseinvoice-update.md)|[purchaseInvoice](../resources/purchaseinvoice.md)|Update the properties of a [purchaseInvoice](../resources/purchaseinvoice.md) object.|
|[post](../api/purchaseinvoice-post.md)|None||
|[List purchaseInvoiceLines](../api/purchaseinvoice-list-purchaseinvoicelines.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md) collection|Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property.|
|[Add purchaseInvoiceLines](../api/purchaseinvoice-post-purchaseinvoicelines.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Add purchaseInvoiceLines by posting to the purchaseInvoiceLines collection.|
|[Get vendor](../api/vendor-get.md)|[vendor](../resources/vendor.md)|Read properties and relationships of the [vendor](../resources/vendor.md) object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read properties and relationships of the [currency](../resources/currency.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|buyFromAddress|[postalAddressType](../resources/postaladdresstype.md)||
|currencyCode|String||
|currencyId|Guid||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|dueDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceDate|Date||
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|payToAddress|[postalAddressType](../resources/postaladdresstype.md)||
|payToContact|String||
|payToName|String||
|payToVendorId|Guid||
|payToVendorNumber|String||
|pricesIncludeTax|Boolean||
|shipToAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shipToContact|String||
|shipToName|String||
|status|String||
|totalAmountExcludingTax|Decimal||
|totalAmountIncludingTax|Decimal||
|totalTaxAmount|Decimal||
|vendorId|Guid||
|vendorInvoiceNumber|String||
|vendorName|String||
|vendorNumber|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)||
|purchaseInvoiceLines|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md) collection||
|vendor|[vendor](../resources/vendor.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.purchaseInvoice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.purchaseInvoice",
  "id": "String (identifier)",
  "number": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "vendorInvoiceNumber": "String",
  "vendorId": "Guid",
  "vendorNumber": "String",
  "vendorName": "String",
  "payToName": "String",
  "payToContact": "String",
  "payToVendorId": "Guid",
  "payToVendorNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "buyFromAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "payToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shipToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

