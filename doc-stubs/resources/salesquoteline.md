---
title: "salesQuoteLine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesQuoteLine resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List item](../api/salesquoteline-list-item.md)|[item](../resources/item.md) collection|Get the items from the item navigation property.|
|[Create item](../api/salesquoteline-post-item.md)|[item](../resources/item.md)|Create a new item object.|
|[Delete item](../api/salesquoteline-delete-item.md)|None|Delete an [item](../resources/item.md) object.|
|[Update item](../api/salesquoteline-update-item.md)|[item](../resources/item.md)|Update the properties of an item object.|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read the properties and relationships of an [item](../resources/item.md) object.|
|[List account](../api/salesquoteline-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/salesquoteline-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/salesquoteline-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/salesquoteline-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read the properties and relationships of an [account](../resources/account.md) object.|
|[List salesQuoteLines](../api/company-list-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md) collection|Get the salesQuoteLines from the salesQuoteLines navigation property.|
|[Create salesQuoteLines](../api/company-post-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md)|Create a new salesQuoteLines object.|

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
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|
|item|[item](../resources/item.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesQuoteLine",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "id": "String (identifier)",
  "documentId": "Guid",
  "sequence": "Integer",
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal",
  "quantity": "Decimal",
  "discountAmount": "Decimal",
  "discountPercent": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "amountExcludingTax": "Decimal",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "amountIncludingTax": "Decimal",
  "netAmount": "Decimal",
  "netTaxAmount": "Decimal",
  "netAmountIncludingTax": "Decimal"
}
```

