---
title: "purchaseInvoice resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# purchaseInvoice resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[post](../api/purchaseinvoice-post.md)|None|**TODO: Add Description**|
|[List purchaseInvoiceLines](../api/purchaseinvoice-list-purchaseinvoicelines.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md) collection|Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property.|
|[Create purchaseInvoiceLines](../api/purchaseinvoice-post-purchaseinvoicelines.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Create a new purchaseInvoiceLines object.|
|[Delete purchaseInvoiceLines](../api/purchaseinvoice-delete-purchaseinvoicelines.md)|None|Delete a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[Update purchaseInvoiceLines](../api/purchaseinvoice-update-purchaseinvoicelines.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Update the properties of a purchaseInvoiceLines object.|
|[Get purchaseInvoiceLine](../api/purchaseinvoiceline-get.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Read the properties and relationships of a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[List vendor](../api/purchaseinvoice-list-vendor.md)|[vendor](../resources/vendor.md) collection|Get the vendors from the vendor navigation property.|
|[Create vendor](../api/purchaseinvoice-post-vendor.md)|[vendor](../resources/vendor.md)|Create a new vendor object.|
|[Delete vendor](../api/purchaseinvoice-delete-vendor.md)|None|Delete a [vendor](../resources/vendor.md) object.|
|[Update vendor](../api/purchaseinvoice-update-vendor.md)|[vendor](../resources/vendor.md)|Update the properties of a vendor object.|
|[Get vendor](../api/vendor-get.md)|[vendor](../resources/vendor.md)|Read the properties and relationships of a [vendor](../resources/vendor.md) object.|
|[List currency](../api/purchaseinvoice-list-currency.md)|[currency](../resources/currency.md) collection|Get the currencies from the currency navigation property.|
|[Create currency](../api/purchaseinvoice-post-currency.md)|[currency](../resources/currency.md)|Create a new currency object.|
|[Delete currency](../api/purchaseinvoice-delete-currency.md)|None|Delete a [currency](../resources/currency.md) object.|
|[Update currency](../api/purchaseinvoice-update-currency.md)|[currency](../resources/currency.md)|Update the properties of a currency object.|
|[Get currency](../api/currency-get.md)|[currency](../resources/currency.md)|Read the properties and relationships of a [currency](../resources/currency.md) object.|
|[List purchaseInvoices](../api/company-list-purchaseinvoices.md)|[purchaseInvoice](../resources/purchaseinvoice.md) collection|Get the purchaseInvoices from the purchaseInvoices navigation property.|
|[Create purchaseInvoices](../api/company-post-purchaseinvoices.md)|[purchaseInvoice](../resources/purchaseinvoice.md)|Create a new purchaseInvoices object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|buyFromAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceDate|Date|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|payToAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|payToContact|String|**TODO: Add Description**|
|payToName|String|**TODO: Add Description**|
|payToVendorId|Guid|**TODO: Add Description**|
|payToVendorNumber|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|shipToAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shipToContact|String|**TODO: Add Description**|
|shipToName|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|vendorId|Guid|**TODO: Add Description**|
|vendorInvoiceNumber|String|**TODO: Add Description**|
|vendorName|String|**TODO: Add Description**|
|vendorNumber|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|currency|[currency](../resources/currency.md)|**TODO: Add Description**|
|purchaseInvoiceLines|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md) collection|**TODO: Add Description**|
|vendor|[vendor](../resources/vendor.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

