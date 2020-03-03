---
title: "purchaseInvoiceLine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# purchaseInvoiceLine resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List purchaseInvoiceLines](../api/purchaseinvoiceline-list.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md) collection|List properties and relationships of the [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) objects.|
|[Get purchaseInvoiceLine](../api/purchaseinvoiceline-get.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Read properties and relationships of the [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[Create purchaseInvoiceLine](../api/purchaseinvoiceline-create.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Create a new [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[Delete purchaseInvoiceLine](../api/purchaseinvoiceline-delete.md)|None|Deletes a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md).|
|[Update purchaseInvoiceLine](../api/purchaseinvoiceline-update.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Update the properties of a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read properties and relationships of the [item](../resources/item.md) object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid||
|amountExcludingTax|Decimal||
|amountIncludingTax|Decimal||
|description|String||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|discountPercent|Decimal||
|documentId|Guid||
|expectedReceiptDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceDiscountAllocation|Decimal||
|itemId|Guid||
|lineType|String||
|netAmount|Decimal||
|netAmountIncludingTax|Decimal||
|netTaxAmount|Decimal||
|quantity|Decimal||
|sequence|Int32||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|unitCost|Decimal||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)||
|item|[item](../resources/item.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.purchaseInvoiceLine",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
  "id": "String (identifier)",
  "documentId": "Guid",
  "sequence": 1024,
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitCost": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "String",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "invoiceDiscountAllocation": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2",
  "expectedReceiptDate": "Date"
}
```

