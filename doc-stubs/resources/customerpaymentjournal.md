---
title: "customerPaymentJournal resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# customerPaymentJournal resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List customerPayments](../api/customerpaymentjournal-list-customerpayments.md)|[customerPayment](../resources/customerpayment.md) collection|Get the customerPayments from the customerPayments navigation property.|
|[Create customerPayments](../api/customerpaymentjournal-post-customerpayments.md)|[customerPayment](../resources/customerpayment.md)|Create a new customerPayments object.|
|[Delete customerPayments](../api/customerpaymentjournal-delete-customerpayments.md)|None|Delete a [customerPayment](../resources/customerpayment.md) object.|
|[Update customerPayments](../api/customerpaymentjournal-update-customerpayments.md)|[customerPayment](../resources/customerpayment.md)|Update the properties of a customerPayments object.|
|[Get customerPayment](../api/customerpayment-get.md)|[customerPayment](../resources/customerpayment.md)|Read the properties and relationships of a [customerPayment](../resources/customerpayment.md) object.|
|[List account](../api/customerpaymentjournal-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/customerpaymentjournal-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/customerpaymentjournal-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/customerpaymentjournal-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read the properties and relationships of an [account](../resources/account.md) object.|
|[List customerPaymentJournals](../api/company-list-customerpaymentjournals.md)|[customerPaymentJournal](../resources/customerpaymentjournal.md) collection|Get the customerPaymentJournals from the customerPaymentJournals navigation property.|
|[Create customerPaymentJournals](../api/company-post-customerpaymentjournals.md)|[customerPaymentJournal](../resources/customerpaymentjournal.md)|Create a new customerPaymentJournals object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|balancingAccountId|Guid|**TODO: Add Description**|
|balancingAccountNumber|String|**TODO: Add Description**|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|
|customerPayments|[customerPayment](../resources/customerpayment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

