---
title: "customerPaymentJournal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# customerPaymentJournal resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get customerPaymentJournal](../api/customerpaymentjournal-get.md)|[customerPaymentJournal](../resources/customerpaymentjournal.md)|Read properties and relationships of the [customerPaymentJournal](../resources/customerpaymentjournal.md) object.|
|[Update customerPaymentJournal](../api/customerpaymentjournal-update.md)|[customerPaymentJournal](../resources/customerpaymentjournal.md)|Update the properties of a [customerPaymentJournal](../resources/customerpaymentjournal.md) object.|
|[List customerPayments](../api/customerpaymentjournal-list-customerpayments.md)|[customerPayment](../resources/customerpayment.md) collection|Get the customerPayments from the customerPayments navigation property.|
|[Add customerPayments](../api/customerpaymentjournal-post-customerpayments.md)|[customerPayment](../resources/customerpayment.md)|Add customerPayments by posting to the customerPayments collection.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|balancingAccountId|Guid||
|balancingAccountNumber|String||
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)||
|customerPayments|[customerPayment](../resources/customerpayment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customerPaymentJournal",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customerPaymentJournal",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```

