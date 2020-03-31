---
title: "salesOrderLine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# salesOrderLine resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesOrderLine](../api/salesorderline-get.md)|[salesOrderLine](../resources/salesorderline.md)|Read properties and relationships of the [salesOrderLine](../resources/salesorderline.md) object.|
|[Update salesOrderLine](../api/salesorderline-update.md)|[salesOrderLine](../resources/salesorderline.md)|Update the properties of a [salesOrderLine](../resources/salesorderline.md) object.|
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
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceDiscountAllocation|Decimal||
|invoicedQuantity|Decimal||
|invoiceQuantity|Decimal||
|itemId|Guid||
|lineType|String||
|netAmount|Decimal||
|netAmountIncludingTax|Decimal||
|netTaxAmount|Decimal||
|quantity|Decimal||
|sequence|Int32||
|shipmentDate|Date||
|shippedQuantity|Decimal||
|shipQuantity|Decimal||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|unitOfMeasureId|Guid||
|unitPrice|Decimal||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)||
|item|[item](../resources/item.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesOrderLine",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "id": "String (identifier)",
  "documentId": "Guid",
  "sequence": 1024,
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitOfMeasureId": "Guid",
  "quantity": "4.2",
  "unitPrice": "4.2",
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
  "shipmentDate": "Date",
  "shippedQuantity": "4.2",
  "invoicedQuantity": "4.2",
  "invoiceQuantity": "4.2",
  "shipQuantity": "4.2"
}
```

