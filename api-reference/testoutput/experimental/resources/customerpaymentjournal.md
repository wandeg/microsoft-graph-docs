---
title: "customerPaymentJournal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# customerPaymentJournal resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get customerPaymentJournal](../api/customerpaymentjournal-get.md)|[customerPaymentJournal](../resources/customerPaymentJournal.md)|Read properties and relationships of the [customerPaymentJournal](../resources/customerpaymentjournal.md) object.|
|[Delete customerPaymentJournal](../api/customerpaymentjournal-delete.md)|None|Deletes a [customerPaymentJournal](../resources/customerpaymentjournal.md).|
|[Update customerPaymentJournal](../api/customerpaymentjournal-update.md)|[customerPaymentJournal](../resources/customerPaymentJournal.md)|Update the properties of a [customerPaymentJournal](../resources/customerpaymentjournal.md) object.|
|[List customerPayments](../api/customerpaymentjournal-list-customerpayments.md)|[customerPayment](../resources/customerPayment.md) collection|Get the customerPayments from the customerPayments navigation property.|
|[Add customerPayments](../api/customerpaymentjournal-post-customerpayments.md)|[customerPayment](../resources/customerPayment.md)|Add customerPayments by posting to the customerPayments collection.|
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
|customerPayments|[customerPayment](../resources/customerPayment.md) collection||

## JSON Representation
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

