---
title: "salesQuoteLine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# salesQuoteLine resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get salesQuoteLine](../api/salesquoteline-get.md)|[salesQuoteLine](../resources/salesquoteline.md)|Read properties and relationships of the [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Update salesQuoteLine](../api/salesquoteline-update.md)|[salesQuoteLine](../resources/salesquoteline.md)|Update the properties of a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read properties and relationships of the [item](../resources/item.md) object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|
|[List salesQuoteLines](../api/company-list-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md) collection|Get the salesQuoteLines from the salesQuoteLines navigation property.|
|[Add salesQuoteLines](../api/company-post-salesquotelines.md)|[salesQuoteLine](../resources/salesquoteline.md)|Add salesQuoteLines by posting to the salesQuoteLines collection.|

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
  "sequence": 1024,
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitOfMeasureId": "Guid",
  "unitPrice": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "String",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2"
}
```

