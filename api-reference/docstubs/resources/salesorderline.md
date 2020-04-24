---
title: "salesOrderLine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesOrderLine resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesOrderLine](../api/salesorderline-get.md)|[salesOrderLine](../resources/salesorderline.md)|Read the properties and relationships of a [salesOrderLine](../resources/salesorderline.md) object.|
|[Update salesOrderLine](../api/salesorderline-update.md)|[salesOrderLine](../resources/salesorderline.md)|Update the properties of a [salesOrderLine](../resources/salesorderline.md) object.|
|[List item](../api/salesorderline-list-item.md)|[item](../resources/item.md) collection|Get the items from the item navigation property.|
|[Create item](../api/salesorderline-post-item.md)|[item](../resources/item.md)|Create a new item object.|
|[Delete item](../api/salesorderline-delete-item.md)|None|Delete an [item](../resources/item.md) object.|
|[Update item](../api/salesorderline-update-item.md)|[item](../resources/item.md)|Update the properties of an item object.|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read the properties and relationships of an [item](../resources/item.md) object.|
|[List account](../api/salesorderline-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/salesorderline-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/salesorderline-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/salesorderline-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read the properties and relationships of an [account](../resources/account.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid|**TODO: Add Description**|
|amountExcludingTax|Decimal|**TODO: Add Description**|
|amountIncludingTax|Decimal|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|documentId|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceDiscountAllocation|Decimal|**TODO: Add Description**|
|invoicedQuantity|Decimal|**TODO: Add Description**|
|invoiceQuantity|Decimal|**TODO: Add Description**|
|itemId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|shipmentDate|Date|**TODO: Add Description**|
|shippedQuantity|Decimal|**TODO: Add Description**|
|shipQuantity|Decimal|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|
|item|[item](../resources/item.md)|**TODO: Add Description**|

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

