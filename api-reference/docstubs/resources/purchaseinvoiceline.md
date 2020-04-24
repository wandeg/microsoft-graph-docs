---
title: "purchaseInvoiceLine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# purchaseInvoiceLine resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get purchaseInvoiceLine](../api/purchaseinvoiceline-get.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Read the properties and relationships of a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[Update purchaseInvoiceLine](../api/purchaseinvoiceline-update.md)|[purchaseInvoiceLine](../resources/purchaseinvoiceline.md)|Update the properties of a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.|
|[List item](../api/purchaseinvoiceline-list-item.md)|[item](../resources/item.md) collection|Get the items from the item navigation property.|
|[Create item](../api/purchaseinvoiceline-post-item.md)|[item](../resources/item.md)|Create a new item object.|
|[Delete item](../api/purchaseinvoiceline-delete-item.md)|None|Delete an [item](../resources/item.md) object.|
|[Update item](../api/purchaseinvoiceline-update-item.md)|[item](../resources/item.md)|Update the properties of an item object.|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read the properties and relationships of an [item](../resources/item.md) object.|
|[List account](../api/purchaseinvoiceline-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/purchaseinvoiceline-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/purchaseinvoiceline-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/purchaseinvoiceline-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
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
|expectedReceiptDate|Date|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceDiscountAllocation|Decimal|**TODO: Add Description**|
|itemId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|unitCost|Decimal|**TODO: Add Description**|

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

